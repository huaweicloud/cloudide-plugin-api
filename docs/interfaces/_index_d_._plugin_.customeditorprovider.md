**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CustomEditorProvider

# Interface: CustomEditorProvider\<T>

Provider for editable custom editors that use a custom document model.

Custom editors use [`CustomDocument`](#CustomDocument) as their document model instead of a [`TextDocument`](#TextDocument).
This gives extensions full control over actions such as edit, save, and backup.

You should use this type of custom editor when dealing with binary files or more complex scenarios. For simple
text based documents, use [`CustomTextEditorProvider`](#CustomTextEditorProvider) instead.

## Type parameters

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`T` | [CustomDocument](_index_d_._plugin_.customdocument.md) | CustomDocument | Type of the custom document returned by this provider.  |

## Hierarchy

* [CustomReadonlyEditorProvider](_index_d_._plugin_.customreadonlyeditorprovider.md)\<T>

  ↳ **CustomEditorProvider**

## Index

### Properties

* [onDidChangeCustomDocument](_index_d_._plugin_.customeditorprovider.md#ondidchangecustomdocument)

### Methods

* [backupCustomDocument](_index_d_._plugin_.customeditorprovider.md#backupcustomdocument)
* [openCustomDocument](_index_d_._plugin_.customeditorprovider.md#opencustomdocument)
* [resolveCustomEditor](_index_d_._plugin_.customeditorprovider.md#resolvecustomeditor)
* [revertCustomDocument](_index_d_._plugin_.customeditorprovider.md#revertcustomdocument)
* [saveCustomDocument](_index_d_._plugin_.customeditorprovider.md#savecustomdocument)
* [saveCustomDocumentAs](_index_d_._plugin_.customeditorprovider.md#savecustomdocumentas)

## Properties

### onDidChangeCustomDocument

• `Readonly` **onDidChangeCustomDocument**: [Event](_index_d_._plugin_.event.md)\<[CustomDocumentEditEvent](_index_d_._plugin_.customdocumenteditevent.md)\<T>> \| [Event](_index_d_._plugin_.event.md)\<[CustomDocumentContentChangeEvent](_index_d_._plugin_.customdocumentcontentchangeevent.md)\<T>>

*Defined in [index.d.ts:7872](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7872)*

Signal that an edit has occurred inside a custom editor.

This event must be fired by your extension whenever an edit happens in a custom editor. An edit can be
anything from changing some text, to cropping an image, to reordering a list. Your extension is free to
define what an edit is and what data is stored on each edit.

Firing `onDidChange` causes VS Code to mark the editors as being dirty. This is cleared when the user either
saves or reverts the file.

Editors that support undo/redo must fire a `CustomDocumentEditEvent` whenever an edit happens. This allows
users to undo and redo the edit using VS Code's standard VS Code keyboard shortcuts. VS Code will also mark
the editor as no longer being dirty if the user undoes all edits to the last saved state.

Editors that support editing but cannot use VS Code's standard undo/redo mechanism must fire a `CustomDocumentContentChangeEvent`.
The only way for a user to clear the dirty state of an editor that does not support undo/redo is to either
`save` or `revert` the file.

An editor should only ever fire `CustomDocumentEditEvent` events, or only ever fire `CustomDocumentContentChangeEvent` events.

## Methods

### backupCustomDocument

▸ **backupCustomDocument**(`document`: T, `context`: [CustomDocumentBackupContext](_index_d_._plugin_.customdocumentbackupcontext.md), `cancellation`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [Thenable](_index_d_.thenable.md)\<[CustomDocumentBackup](_index_d_._plugin_.customdocumentbackup.md)>

*Defined in [index.d.ts:7945](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7945)*

Back up a dirty custom document.

Backups are used for hot exit and to prevent data loss. Your `backup` method should persist the resource in
its current state, i.e. with the edits applied. Most commonly this means saving the resource to disk in
the `ExtensionContext.storagePath`. When VS Code reloads and your custom editor is opened for a resource,
your extension should first check to see if any backups exist for the resource. If there is a backup, your
extension should load the file contents from there instead of from the resource in the workspace.

`backup` is triggered approximately one second after the user stops editing the document. If the user
rapidly edits the document, `backup` will not be invoked until the editing stops.

`backup` is not invoked when `auto save` is enabled (since auto save already persists the resource).

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | T | Document to backup. |
`context` | [CustomDocumentBackupContext](_index_d_._plugin_.customdocumentbackupcontext.md) | Information that can be used to backup the document. |
`cancellation` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | Token that signals the current backup since a new backup is coming in. It is up to your extension to decided how to respond to cancellation. If for example your extension is backing up a large file in an operation that takes time to complete, your extension may decide to finish the ongoing backup rather than cancelling it to ensure that VS Code has some valid backup.  |

**Returns:** [Thenable](_index_d_.thenable.md)\<[CustomDocumentBackup](_index_d_._plugin_.customdocumentbackup.md)>

___

### openCustomDocument

▸ **openCustomDocument**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md), `openContext`: [CustomDocumentOpenContext](_index_d_._plugin_.customdocumentopencontext.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [Thenable](_index_d_.thenable.md)\<T> \| T

*Inherited from [CustomReadonlyEditorProvider](_index_d_._plugin_.customreadonlyeditorprovider.md).[openCustomDocument](_index_d_._plugin_.customreadonlyeditorprovider.md#opencustomdocument)*

*Defined in [index.d.ts:7818](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7818)*

Create a new document for a given resource.

`openCustomDocument` is called when the first time an editor for a given resource is opened. The opened
document is then passed to `resolveCustomEditor` so that the editor can be shown to the user.

Already opened `CustomDocument` are re-used if the user opened additional editors. When all editors for a
given resource are closed, the `CustomDocument` is disposed of. Opening an editor at this point will
trigger another call to `openCustomDocument`.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | Uri of the document to open. |
`openContext` | [CustomDocumentOpenContext](_index_d_._plugin_.customdocumentopencontext.md) | Additional information about the opening custom document. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token that indicates the result is no longer needed.  |

**Returns:** [Thenable](_index_d_.thenable.md)\<T> \| T

The custom document.

___

### resolveCustomEditor

▸ **resolveCustomEditor**(`document`: T, `webviewPanel`: [WebviewPanel](_index_d_._plugin_.webviewpanel.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [Thenable](_index_d_.thenable.md)\<void> \| void

*Inherited from [CustomReadonlyEditorProvider](_index_d_._plugin_.customreadonlyeditorprovider.md).[resolveCustomEditor](_index_d_._plugin_.customreadonlyeditorprovider.md#resolvecustomeditor)*

*Defined in [index.d.ts:7837](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7837)*

Resolve a custom editor for a given resource.

This is called whenever the user opens a new editor for this `CustomEditorProvider`.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | T | Document for the resource being resolved.  |
`webviewPanel` | [WebviewPanel](_index_d_._plugin_.webviewpanel.md) | The webview panel used to display the editor UI for this resource.  During resolve, the provider must fill in the initial html for the content webview panel and hook up all the event listeners on it that it is interested in. The provider can also hold onto the `WebviewPanel` to use later for example in a command. See [`WebviewPanel`](#WebviewPanel) for additional details.  |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token that indicates the result is no longer needed.  |

**Returns:** [Thenable](_index_d_.thenable.md)\<void> \| void

Optional thenable indicating that the custom editor has been resolved.

___

### revertCustomDocument

▸ **revertCustomDocument**(`document`: T, `cancellation`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [Thenable](_index_d_.thenable.md)\<void>

*Defined in [index.d.ts:7922](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7922)*

Revert a custom document to its last saved state.

This method is invoked by VS Code when the user triggers `File: Revert File` in a custom editor. (Note that
this is only used using VS Code's `File: Revert File` command and not on a `git revert` of the file).

To implement `revert`, the implementer must make sure all editor instances (webviews) for `document`
are displaying the document in the same state is saved in. This usually means reloading the file from the
workspace.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | T | Document to revert. |
`cancellation` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | Token that signals the revert is no longer required.  |

**Returns:** [Thenable](_index_d_.thenable.md)\<void>

Thenable signaling that the change has completed.

___

### saveCustomDocument

▸ **saveCustomDocument**(`document`: T, `cancellation`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [Thenable](_index_d_.thenable.md)\<void>

*Defined in [index.d.ts:7889](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7889)*

Save a custom document.

This method is invoked by VS Code when the user saves a custom editor. This can happen when the user
triggers save while the custom editor is active, by commands such as `save all`, or by auto save if enabled.

To implement `save`, the implementer must persist the custom editor. This usually means writing the
file data for the custom document to disk. After `save` completes, any associated editor instances will
no longer be marked as dirty.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | T | Document to save. |
`cancellation` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | Token that signals the save is no longer required (for example, if another save was triggered).  |

**Returns:** [Thenable](_index_d_.thenable.md)\<void>

Thenable signaling that saving has completed.

___

### saveCustomDocumentAs

▸ **saveCustomDocumentAs**(`document`: T, `destination`: [Uri](../classes/_index_d_._plugin_.uri.md), `cancellation`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [Thenable](_index_d_.thenable.md)\<void>

*Defined in [index.d.ts:7905](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7905)*

Save a custom document to a different location.

This method is invoked by VS Code when the user triggers 'save as' on a custom editor. The implementer must
persist the custom editor to `destination`.

When the user accepts save as, the current editor is be replaced by an non-dirty editor for the newly saved file.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | T | Document to save. |
`destination` | [Uri](../classes/_index_d_._plugin_.uri.md) | Location to save to. |
`cancellation` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | Token that signals the save is no longer required.  |

**Returns:** [Thenable](_index_d_.thenable.md)\<void>

Thenable signaling that saving has completed.
