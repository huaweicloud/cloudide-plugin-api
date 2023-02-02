[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CustomEditorProvider

# Interface: CustomEditorProvider<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).CustomEditorProvider

Provider for editable custom editors that use a custom document model.

Custom editors use [`CustomDocument`](codearts_plugin_.CustomDocument.md) as their document model instead of a [`TextDocument`](codearts_plugin_.TextDocument.md).
This gives extensions full control over actions such as edit, save, and backup.

You should use this type of custom editor when dealing with binary files or more complex scenarios. For simple
text based documents, use [`CustomTextEditorProvider`](codearts_plugin_.CustomTextEditorProvider.md) instead.

## Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `T` | extends [`CustomDocument`](codearts_plugin_.CustomDocument.md) = [`CustomDocument`](codearts_plugin_.CustomDocument.md) | Type of the custom document returned by this provider. |

## Hierarchy

- [`CustomReadonlyEditorProvider`](codearts_plugin_.CustomReadonlyEditorProvider.md)<`T`\>

  ↳ **`CustomEditorProvider`**

## Table of contents

### Properties

- [onDidChangeCustomDocument](codearts_plugin_.CustomEditorProvider.md#ondidchangecustomdocument)

### Methods

- [backupCustomDocument](codearts_plugin_.CustomEditorProvider.md#backupcustomdocument)
- [openCustomDocument](codearts_plugin_.CustomEditorProvider.md#opencustomdocument)
- [resolveCustomEditor](codearts_plugin_.CustomEditorProvider.md#resolvecustomeditor)
- [revertCustomDocument](codearts_plugin_.CustomEditorProvider.md#revertcustomdocument)
- [saveCustomDocument](codearts_plugin_.CustomEditorProvider.md#savecustomdocument)
- [saveCustomDocumentAs](codearts_plugin_.CustomEditorProvider.md#savecustomdocumentas)

## Properties

### onDidChangeCustomDocument

• `Readonly` **onDidChangeCustomDocument**: [`Event`](codearts_plugin_.Event.md)<[`CustomDocumentEditEvent`](codearts_plugin_.CustomDocumentEditEvent.md)<`T`\>\> \| [`Event`](codearts_plugin_.Event.md)<[`CustomDocumentContentChangeEvent`](codearts_plugin_.CustomDocumentContentChangeEvent.md)<`T`\>\>

Signal that an edit has occurred inside a custom editor.

This event must be fired by your extension whenever an edit happens in a custom editor. An edit can be
anything from changing some text, to cropping an image, to reordering a list. Your extension is free to
define what an edit is and what data is stored on each edit.

Firing `onDidChange` causes the editors to be marked as being dirty. This is cleared when the user either
saves or reverts the file.

Editors that support undo/redo must fire a `CustomDocumentEditEvent` whenever an edit happens. This allows
users to undo and redo the edit using the editor's standard keyboard shortcuts. The editor will also mark
the editor as no longer being dirty if the user undoes all edits to the last saved state.

Editors that support editing but cannot use the editor's standard undo/redo mechanism must fire a `CustomDocumentContentChangeEvent`.
The only way for a user to clear the dirty state of an editor that does not support undo/redo is to either
`save` or `revert` the file.

An editor should only ever fire `CustomDocumentEditEvent` events, or only ever fire `CustomDocumentContentChangeEvent` events.

#### Defined in

[index.d.ts:8989](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8989)

## Methods

### backupCustomDocument

▸ **backupCustomDocument**(`document`, `context`, `cancellation`): [`Thenable`](Thenable.md)<[`CustomDocumentBackup`](codearts_plugin_.CustomDocumentBackup.md)\>

Back up a dirty custom document.

Backups are used for hot exit and to prevent data loss. Your `backup` method should persist the resource in
its current state, i.e. with the edits applied. Most commonly this means saving the resource to disk in
the `ExtensionContext.storagePath`. When the editor reloads and your custom editor is opened for a resource,
your extension should first check to see if any backups exist for the resource. If there is a backup, your
extension should load the file contents from there instead of from the resource in the workspace.

`backup` is triggered approximately one second after the user stops editing the document. If the user
rapidly edits the document, `backup` will not be invoked until the editing stops.

`backup` is not invoked when `auto save` is enabled (since auto save already persists the resource).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | `T` | Document to backup. |
| `context` | [`CustomDocumentBackupContext`](codearts_plugin_.CustomDocumentBackupContext.md) | Information that can be used to backup the document. |
| `cancellation` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | Token that signals the current backup since a new backup is coming in. It is up to your extension to decided how to respond to cancellation. If for example your extension is backing up a large file in an operation that takes time to complete, your extension may decide to finish the ongoing backup rather than cancelling it to ensure that the editor has some valid backup. |

#### Returns

[`Thenable`](Thenable.md)<[`CustomDocumentBackup`](codearts_plugin_.CustomDocumentBackup.md)\>

#### Defined in

[index.d.ts:9062](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9062)

___

### openCustomDocument

▸ **openCustomDocument**(`uri`, `openContext`, `token`): `T` \| [`Thenable`](Thenable.md)<`T`\>

Create a new document for a given resource.

`openCustomDocument` is called when the first time an editor for a given resource is opened. The opened
document is then passed to `resolveCustomEditor` so that the editor can be shown to the user.

Already opened `CustomDocument` are re-used if the user opened additional editors. When all editors for a
given resource are closed, the `CustomDocument` is disposed of. Opening an editor at this point will
trigger another call to `openCustomDocument`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | Uri of the document to open. |
| `openContext` | [`CustomDocumentOpenContext`](codearts_plugin_.CustomDocumentOpenContext.md) | Additional information about the opening custom document. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token that indicates the result is no longer needed. |

#### Returns

`T` \| [`Thenable`](Thenable.md)<`T`\>

The custom document.

#### Inherited from

[CustomReadonlyEditorProvider](codearts_plugin_.CustomReadonlyEditorProvider.md).[openCustomDocument](codearts_plugin_.CustomReadonlyEditorProvider.md#opencustomdocument)

#### Defined in

[index.d.ts:8935](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8935)

___

### resolveCustomEditor

▸ **resolveCustomEditor**(`document`, `webviewPanel`, `token`): `void` \| [`Thenable`](Thenable.md)<`void`\>

Resolve a custom editor for a given resource.

This is called whenever the user opens a new editor for this `CustomEditorProvider`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | `T` | Document for the resource being resolved. |
| `webviewPanel` | [`WebviewPanel`](codearts_plugin_.WebviewPanel.md) | The webview panel used to display the editor UI for this resource.  During resolve, the provider must fill in the initial html for the content webview panel and hook up all the event listeners on it that it is interested in. The provider can also hold onto the `WebviewPanel` to use later for example in a command. See [`WebviewPanel`](codearts_plugin_.WebviewPanel.md) for additional details. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token that indicates the result is no longer needed. |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

Optional thenable indicating that the custom editor has been resolved.

#### Inherited from

[CustomReadonlyEditorProvider](codearts_plugin_.CustomReadonlyEditorProvider.md).[resolveCustomEditor](codearts_plugin_.CustomReadonlyEditorProvider.md#resolvecustomeditor)

#### Defined in

[index.d.ts:8954](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8954)

___

### revertCustomDocument

▸ **revertCustomDocument**(`document`, `cancellation`): [`Thenable`](Thenable.md)<`void`\>

Revert a custom document to its last saved state.

This method is invoked by the editor when the user triggers `File: Revert File` in a custom editor. (Note that
this is only used using the editor's `File: Revert File` command and not on a `git revert` of the file).

To implement `revert`, the implementer must make sure all editor instances (webviews) for `document`
are displaying the document in the same state is saved in. This usually means reloading the file from the
workspace.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | `T` | Document to revert. |
| `cancellation` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | Token that signals the revert is no longer required. |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

Thenable signaling that the change has completed.

#### Defined in

[index.d.ts:9039](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9039)

___

### saveCustomDocument

▸ **saveCustomDocument**(`document`, `cancellation`): [`Thenable`](Thenable.md)<`void`\>

Save a custom document.

This method is invoked by the editor when the user saves a custom editor. This can happen when the user
triggers save while the custom editor is active, by commands such as `save all`, or by auto save if enabled.

To implement `save`, the implementer must persist the custom editor. This usually means writing the
file data for the custom document to disk. After `save` completes, any associated editor instances will
no longer be marked as dirty.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | `T` | Document to save. |
| `cancellation` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | Token that signals the save is no longer required (for example, if another save was triggered). |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

Thenable signaling that saving has completed.

#### Defined in

[index.d.ts:9006](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9006)

___

### saveCustomDocumentAs

▸ **saveCustomDocumentAs**(`document`, `destination`, `cancellation`): [`Thenable`](Thenable.md)<`void`\>

Save a custom document to a different location.

This method is invoked by the editor when the user triggers 'save as' on a custom editor. The implementer must
persist the custom editor to `destination`.

When the user accepts save as, the current editor is be replaced by an non-dirty editor for the newly saved file.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | `T` | Document to save. |
| `destination` | [`Uri`](../classes/codearts_plugin_.Uri.md) | Location to save to. |
| `cancellation` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | Token that signals the save is no longer required. |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

Thenable signaling that saving has completed.

#### Defined in

[index.d.ts:9022](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9022)
