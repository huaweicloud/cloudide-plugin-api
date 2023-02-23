[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](_cloudide_plugin_.md) / workspace

# Namespace: workspace

["@cloudide/plugin"](_cloudide_plugin_.md).workspace

Namespace for dealing with the current workspace. A workspace is the representation
of the folder that has been opened. There is no workspace when just a file but not a
folder has been opened.

The workspace offers support for [listening](#workspace.createFileSystemWatcher) to fs
events and for [finding](#workspace.findFiles) files. Both perform well and run _outside_
the editor-process so that they should be always used instead of nodejs-equivalents.

## Table of contents

### Variables

- [fs](cloudide_plugin_.workspace.md#fs)
- [name](cloudide_plugin_.workspace.md#name)
- [rootPath](cloudide_plugin_.workspace.md#rootpath)
- [textDocuments](cloudide_plugin_.workspace.md#textdocuments)
- [workspaceFile](cloudide_plugin_.workspace.md#workspacefile)
- [workspaceFolders](cloudide_plugin_.workspace.md#workspacefolders)

### Functions

- [applyEdit](cloudide_plugin_.workspace.md#applyedit)
- [asRelativePath](cloudide_plugin_.workspace.md#asrelativepath)
- [createFileSystemWatcher](cloudide_plugin_.workspace.md#createfilesystemwatcher)
- [findFiles](cloudide_plugin_.workspace.md#findfiles)
- [findTextInFiles](cloudide_plugin_.workspace.md#findtextinfiles)
- [getConfiguration](cloudide_plugin_.workspace.md#getconfiguration)
- [getWorkspaceFolder](cloudide_plugin_.workspace.md#getworkspacefolder)
- [onDidChangeConfiguration](cloudide_plugin_.workspace.md#ondidchangeconfiguration)
- [onDidChangeTextDocument](cloudide_plugin_.workspace.md#ondidchangetextdocument)
- [onDidChangeWorkspaceFolders](cloudide_plugin_.workspace.md#ondidchangeworkspacefolders)
- [onDidCloseTextDocument](cloudide_plugin_.workspace.md#ondidclosetextdocument)
- [onDidCreateFiles](cloudide_plugin_.workspace.md#ondidcreatefiles)
- [onDidDeleteFiles](cloudide_plugin_.workspace.md#ondiddeletefiles)
- [onDidOpenTextDocument](cloudide_plugin_.workspace.md#ondidopentextdocument)
- [onDidRenameFiles](cloudide_plugin_.workspace.md#ondidrenamefiles)
- [onDidSaveTextDocument](cloudide_plugin_.workspace.md#ondidsavetextdocument)
- [onWillCreateFiles](cloudide_plugin_.workspace.md#onwillcreatefiles)
- [onWillDeleteFiles](cloudide_plugin_.workspace.md#onwilldeletefiles)
- [onWillRenameFiles](cloudide_plugin_.workspace.md#onwillrenamefiles)
- [onWillSaveTextDocument](cloudide_plugin_.workspace.md#onwillsavetextdocument)
- [openTextDocument](cloudide_plugin_.workspace.md#opentextdocument)
- [registerFileSystemProvider](cloudide_plugin_.workspace.md#registerfilesystemprovider)
- [registerTaskProvider](cloudide_plugin_.workspace.md#registertaskprovider)
- [registerTextDocumentContentProvider](cloudide_plugin_.workspace.md#registertextdocumentcontentprovider)
- [saveAll](cloudide_plugin_.workspace.md#saveall)
- [updateWorkspaceFolders](cloudide_plugin_.workspace.md#updateworkspacefolders)

## Variables

### fs

• `Const` **fs**: [`FileSystem`](../interfaces/cloudide_plugin_.FileSystem.md)

A [file system](#FileSystem) instance that allows to interact with local and remote
files, e.g. `workspace.fs.readDirectory(someUri)` allows to retrieve all entries
of a directory or `workspace.fs.stat(anotherUri)` returns the meta data for a
file.

#### Defined in

[index.d.ts:5977](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5977)

___

### name

• `Readonly` **name**: `string` \| `undefined`

The name of the workspace. `undefined` when no folder
has been opened.

#### Defined in

[index.d.ts:6019](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6019)

___

### rootPath

• `Readonly` **rootPath**: `string` \| `undefined`

~~The folder that is open in the editor. `undefined` when no folder
has been opened.~~

**`Deprecated`**

Use [`workspaceFolders`](#workspace.workspaceFolders) instead.

#### Defined in

[index.d.ts:5987](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5987)

___

### textDocuments

• `Readonly` **textDocuments**: [`TextDocument`](../interfaces/cloudide_plugin_.TextDocument.md)[]

All text documents currently known to the system.

#### Defined in

[index.d.ts:6031](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6031)

___

### workspaceFile

• `Const` `Readonly` **workspaceFile**: [`Uri`](../classes/cloudide_plugin_.Uri.md) \| `undefined`

The location of the workspace file, for example:

`file:///Users/name/Development/myProject.code-workspace`

Depending on the workspace that is opened, the value will be:
 * `undefined` when no workspace or a single folder is opened
 * the path of the workspace file as `Uri` otherwise.

**Note:** it is not advised to use `workspace.workspaceFile` to write
configuration data into the file.

#### Defined in

[index.d.ts:6011](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6011)

___

### workspaceFolders

• `Readonly` **workspaceFolders**: [`WorkspaceFolder`](../interfaces/cloudide_plugin_.WorkspaceFolder.md)[] \| `undefined`

List of workspace folders or `undefined` when no folder is open.
*Note* that the first entry corresponds to the value of `rootPath`.

#### Defined in

[index.d.ts:5995](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5995)

## Functions

### applyEdit

▸ **applyEdit**(`edit`): `PromiseLike`<`boolean`\>

Make changes to one or many resources or create, delete, and rename resources as defined by the given
[workspace edit](#WorkspaceEdit).

All changes of a workspace edit are applied in the same order in which they have been added. If
multiple textual inserts are made at the same position, these strings appear in the resulting text
in the order the 'inserts' were made. Invalid sequences like 'delete file a' -> 'insert text in file a'
cause failure of the operation.

When applying a workspace edit that consists only of text edits an 'all-or-nothing'-strategy is used.
A workspace edit with resource creations or deletions aborts the operation, e.g. consecutive edits will
not be attempted, when a single edit fails.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `edit` | [`WorkspaceEdit`](../classes/cloudide_plugin_.WorkspaceEdit.md) | A workspace edit. |

#### Returns

`PromiseLike`<`boolean`\>

A thenable that resolves when the edit could be applied.

#### Defined in

[index.d.ts:6294](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6294)

___

### asRelativePath

▸ **asRelativePath**(`pathOrUri`, `includeWorkspaceFolder?`): `string` \| `undefined`

Returns a path that is relative to the workspace folder or folders.

When there are no [workspace folders](#workspace.workspaceFolders) or when the path
is not contained in them, the input is returned.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pathOrUri` | `string` \| [`Uri`](../classes/cloudide_plugin_.Uri.md) | A path or uri. When a uri is given its [fsPath](#Uri.fsPath) is used. |
| `includeWorkspaceFolder?` | `boolean` | When `true` and when the given path is contained inside a workspace folder the name of the workspace is prepended. Defaults to `true` when there are multiple workspace folders and `false` otherwise. |

#### Returns

`string` \| `undefined`

A path relative to the root or the input.

#### Defined in

[index.d.ts:6330](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6330)

___

### createFileSystemWatcher

▸ **createFileSystemWatcher**(`globPattern`, `ignoreCreateEvents?`, `ignoreChangeEvents?`, `ignoreDeleteEvents?`): [`FileSystemWatcher`](../interfaces/cloudide_plugin_.FileSystemWatcher.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `globPattern` | [`GlobPattern`](_cloudide_plugin_.md#globpattern) |
| `ignoreCreateEvents?` | `boolean` |
| `ignoreChangeEvents?` | `boolean` |
| `ignoreDeleteEvents?` | `boolean` |

#### Returns

[`FileSystemWatcher`](../interfaces/cloudide_plugin_.FileSystemWatcher.md)

#### Defined in

[index.d.ts:6236](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6236)

___

### findFiles

▸ **findFiles**(`include`, `exclude?`, `maxResults?`, `token?`): `PromiseLike`<[`Uri`](../classes/cloudide_plugin_.Uri.md)[]\>

Find files across all [workspace folders](#workspace.workspaceFolders) in the workspace.

**`Sample`**

`findFiles('**​/*.js', '**​/node_modules/**', 10)`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `include` | [`GlobPattern`](_cloudide_plugin_.md#globpattern) | A [glob pattern](#GlobPattern) that defines the files to search for. The glob pattern will be matched against the file paths of resulting matches relative to their workspace. Use a [relative pattern](#RelativePattern) to restrict the search results to a [workspace folder](#WorkspaceFolder). |
| `exclude?` | ``null`` \| [`GlobPattern`](_cloudide_plugin_.md#globpattern) | A [glob pattern](#GlobPattern) that defines files and folders to exclude. The glob pattern will be matched against the file paths of resulting matches relative to their workspace. When `undefined` only default excludes will apply, when `null` no excludes will apply. |
| `maxResults?` | `number` | An upper-bound for the result. |
| `token?` | [`CancellationToken`](../interfaces/cloudide_plugin_.CancellationToken.md) | A token that can be used to signal cancellation to the underlying search engine. |

#### Returns

`PromiseLike`<[`Uri`](../classes/cloudide_plugin_.Uri.md)[]\>

A thenable that resolves to an array of resource identifiers. Will return no results if no
[workspace folders](#workspace.workspaceFolders) are opened.

#### Defined in

[index.d.ts:6258](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6258)

___

### findTextInFiles

▸ **findTextInFiles**(`query`, `optionsOrCallback`, `callbackOrToken?`, `token?`): `Promise`<`TextSearchComplete`\>

Find text in files across all [workspace folders] in the workspace

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `query` | `TextSearchQuery` | What to search |
| `optionsOrCallback` | `any` |  |
| `callbackOrToken?` | [`CancellationToken`](../interfaces/cloudide_plugin_.CancellationToken.md) \| (`result`: `TextSearchResult`) => `void` |  |
| `token?` | [`CancellationToken`](../interfaces/cloudide_plugin_.CancellationToken.md) |  |

#### Returns

`Promise`<`TextSearchComplete`\>

#### Defined in

[index.d.ts:6267](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6267)

___

### getConfiguration

▸ **getConfiguration**(`section?`, `resource?`): [`WorkspaceConfiguration`](../interfaces/cloudide_plugin_.WorkspaceConfiguration.md)

Get a workspace configuration object.

When a section-identifier is provided only that part of the configuration
is returned. Dots in the section-identifier are interpreted as child-access,
like `{ myExt: { setting: { doIt: true }}}` and `getConfiguration('myExt.setting').get('doIt') === true`.

When a resource is provided, configuration scoped to that resource is returned.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `section?` | `string` | A dot-separated identifier. |
| `resource?` | ``null`` \| [`Uri`](../classes/cloudide_plugin_.Uri.md) | A resource for which the configuration is asked for |

#### Returns

[`WorkspaceConfiguration`](../interfaces/cloudide_plugin_.WorkspaceConfiguration.md)

The full configuration or a subset.

#### Defined in

[index.d.ts:6214](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6214)

___

### getWorkspaceFolder

▸ **getWorkspaceFolder**(`uri`): [`WorkspaceFolder`](../interfaces/cloudide_plugin_.WorkspaceFolder.md) \| `undefined`

Returns the [workspace folder](#WorkspaceFolder) that contains a given uri.
* returns `undefined` when the given uri doesn't match any workspace folder

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | An uri. |

#### Returns

[`WorkspaceFolder`](../interfaces/cloudide_plugin_.WorkspaceFolder.md) \| `undefined`

A workspace folder or `undefined`

#### Defined in

[index.d.ts:6316](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6316)

___

### onDidChangeConfiguration

▸ **onDidChangeConfiguration**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`ConfigurationChangeEvent`](../interfaces/cloudide_plugin_.ConfigurationChangeEvent.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidChangeTextDocument

▸ **onDidChangeTextDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TextDocumentChangeEvent`](../interfaces/cloudide_plugin_.TextDocumentChangeEvent.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidChangeWorkspaceFolders

▸ **onDidChangeWorkspaceFolders**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`WorkspaceFoldersChangeEvent`](../interfaces/cloudide_plugin_.WorkspaceFoldersChangeEvent.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidCloseTextDocument

▸ **onDidCloseTextDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TextDocument`](../interfaces/cloudide_plugin_.TextDocument.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidCreateFiles

▸ **onDidCreateFiles**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`FileCreateEvent`](../interfaces/cloudide_plugin_.FileCreateEvent.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidDeleteFiles

▸ **onDidDeleteFiles**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`FileDeleteEvent`](../interfaces/cloudide_plugin_.FileDeleteEvent.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidOpenTextDocument

▸ **onDidOpenTextDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TextDocument`](../interfaces/cloudide_plugin_.TextDocument.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidRenameFiles

▸ **onDidRenameFiles**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`FileRenameEvent`](../interfaces/cloudide_plugin_.FileRenameEvent.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidSaveTextDocument

▸ **onDidSaveTextDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TextDocument`](../interfaces/cloudide_plugin_.TextDocument.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onWillCreateFiles

▸ **onWillCreateFiles**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`FileWillCreateEvent`](../interfaces/cloudide_plugin_.FileWillCreateEvent.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onWillDeleteFiles

▸ **onWillDeleteFiles**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`FileWillDeleteEvent`](../interfaces/cloudide_plugin_.FileWillDeleteEvent.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onWillRenameFiles

▸ **onWillRenameFiles**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`FileWillRenameEvent`](../interfaces/cloudide_plugin_.FileWillRenameEvent.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onWillSaveTextDocument

▸ **onWillSaveTextDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TextDocumentWillSaveEvent`](../interfaces/cloudide_plugin_.TextDocumentWillSaveEvent.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### openTextDocument

▸ **openTextDocument**(`uri`): `PromiseLike`<[`TextDocument`](../interfaces/cloudide_plugin_.TextDocument.md) \| `undefined`\>

Opens a document. Will return early if this document is already open. Otherwise
the document is loaded and the [didOpen](#workspace.onDidOpenTextDocument)-event fires.

The document is denoted by an [uri](#Uri). Depending on the [scheme](#Uri.scheme) the
following rules apply:
* `file`-scheme: Open a file on disk, will be rejected if the file does not exist or cannot be loaded.
* `untitled`-scheme: A new file that should be saved on disk, e.g. `untitled:c:\frodo\new.js`. The language
will be derived from the file name.
* For all other schemes the registered text document content [providers](#TextDocumentContentProvider) are consulted.

*Note* that the lifecycle of the returned document is owned by the editor and not by the extension. That means an
[`onDidClose`](#workspace.onDidCloseTextDocument)-event can occur at any time after opening it.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | Identifies the resource to open. |

#### Returns

`PromiseLike`<[`TextDocument`](../interfaces/cloudide_plugin_.TextDocument.md) \| `undefined`\>

A promise that resolves to a [document](#TextDocument).

#### Defined in

[index.d.ts:6180](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6180)

▸ **openTextDocument**(`fileName`): `PromiseLike`<[`TextDocument`](../interfaces/cloudide_plugin_.TextDocument.md) \| `undefined`\>

A short-hand for `openTextDocument(Uri.file(fileName))`.

**`See`**

[openTextDocument](#openTextDocument)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fileName` | `string` | A name of a file on disk. |

#### Returns

`PromiseLike`<[`TextDocument`](../interfaces/cloudide_plugin_.TextDocument.md) \| `undefined`\>

A promise that resolves to a [document](#TextDocument).

#### Defined in

[index.d.ts:6189](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6189)

▸ **openTextDocument**(`options?`): `PromiseLike`<[`TextDocument`](../interfaces/cloudide_plugin_.TextDocument.md) \| `undefined`\>

Opens an untitled text document. The editor will prompt the user for a file
path when the document is to be saved. The `options` parameter allows to
specify the *language* and/or the *content* of the document.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | `Object` | Options to control how the document will be created. |
| `options.content?` | `string` | - |
| `options.language?` | `string` | - |

#### Returns

`PromiseLike`<[`TextDocument`](../interfaces/cloudide_plugin_.TextDocument.md) \| `undefined`\>

A promise that resolves to a [document](#TextDocument).

#### Defined in

[index.d.ts:6199](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6199)

___

### registerFileSystemProvider

▸ **registerFileSystemProvider**(`scheme`, `provider`, `options?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a filesystem provider for a given scheme, e.g. `ftp`.

There can only be one provider per scheme and an error is being thrown when a scheme
has been claimed by another provider or when it is reserved.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scheme` | `string` | The uri-[scheme](#Uri.scheme) the provider registers for. |
| `provider` | [`FileSystemProvider`](../interfaces/cloudide_plugin_.FileSystemProvider.md) | The filesystem provider. |
| `options?` | `Object` | Immutable metadata about the provider. |
| `options.isCaseSensitive?` | `boolean` | - |
| `options.isReadonly?` | `boolean` | - |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:6307](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6307)

___

### registerTaskProvider

▸ **registerTaskProvider**(`type`, `provider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

~~Register a task provider.~~

**`Deprecated`**

Use the corresponding function on the `tasks` namespace instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `string` | The task kind type this provider is registered for. |
| `provider` | [`TaskProvider`](../interfaces/cloudide_plugin_.TaskProvider.md)<[`Task`](../classes/cloudide_plugin_.Task.md)\> | A task provider. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:6384](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6384)

___

### registerTextDocumentContentProvider

▸ **registerTextDocumentContentProvider**(`scheme`, `provider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a text document content provider.

Only one provider can be registered per scheme.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scheme` | `string` | The uri-scheme to register for. |
| `provider` | [`TextDocumentContentProvider`](../interfaces/cloudide_plugin_.TextDocumentContentProvider.md) | A content provider. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:6042](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6042)

___

### saveAll

▸ **saveAll**(`includeUntitled?`): `PromiseLike`<`boolean`\>

Save all dirty files.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `includeUntitled?` | `boolean` | Also save files that have been created during this session. |

#### Returns

`PromiseLike`<`boolean`\>

A thenable that resolves when the files have been saved.

#### Defined in

[index.d.ts:6276](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6276)

___

### updateWorkspaceFolders

▸ **updateWorkspaceFolders**(`start`, `deleteCount`, `...workspaceFoldersToAdd`): `boolean`

This method replaces `deleteCount` [workspace folders](#workspace.workspaceFolders) starting at index `start`
by an optional set of `workspaceFoldersToAdd` on the `theia.workspace.workspaceFolders` array. This "splice"
behavior can be used to add, remove and change workspace folders in a single operation.

If the first workspace folder is added, removed or changed, the currently executing extensions (including the
one that called this method) will be terminated and restarted so that the (deprecated) `rootPath` property is
updated to point to the first workspace folder.

Use the [`onDidChangeWorkspaceFolders()`](#onDidChangeWorkspaceFolders) event to get notified when the
workspace folders have been updated.

**Example:** adding a new workspace folder at the end of workspace folders
```typescript
workspace.updateWorkspaceFolders(workspace.workspaceFolders ? workspace.workspaceFolders.length : 0, null, { uri: ...});
```

**Example:** removing the first workspace folder
```typescript
workspace.updateWorkspaceFolders(0, 1);
```

**Example:** replacing an existing workspace folder with a new one
```typescript
workspace.updateWorkspaceFolders(0, 1, { uri: ...});
```

It is valid to remove an existing workspace folder and add it again with a different name
to rename that folder.

**Note:** it is not valid to call [updateWorkspaceFolders()](#updateWorkspaceFolders) multiple times
without waiting for the [`onDidChangeWorkspaceFolders()`](#onDidChangeWorkspaceFolders) to fire.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start` | `number` | the zero-based location in the list of currently opened [workspace folders](#WorkspaceFolder) from which to start deleting workspace folders. |
| `deleteCount` | `undefined` \| ``null`` \| `number` | the optional number of workspace folders to remove. |
| `...workspaceFoldersToAdd` | { `name?`: `string` ; `uri`: [`Uri`](../classes/cloudide_plugin_.Uri.md)  }[] | the optional variable set of workspace folders to add in place of the deleted ones. Each workspace is identified with a mandatory URI and an optional name. |

#### Returns

`boolean`

true if the operation was successfully started and false otherwise if arguments were used that would result
in invalid workspace folder state (e.g. 2 folders with the same URI).

#### Defined in

[index.d.ts:6373](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6373)
