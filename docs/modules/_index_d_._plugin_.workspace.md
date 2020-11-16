**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](_index_d_.md) / ["plugin"](_index_d_._plugin_.md) / workspace

# Namespace: workspace

Namespace for dealing with the current workspace. A workspace is the representation
of the folder that has been opened. There is no workspace when just a file but not a
folder has been opened.

The workspace offers support for [listening](#workspace.createFileSystemWatcher) to fs
events and for [finding](#workspace.findFiles) files. Both perform well and run _outside_
the editor-process so that they should be always used instead of nodejs-equivalents.

## Index

### Variables

* [fs](_index_d_._plugin_.workspace.md#fs)
* [name](_index_d_._plugin_.workspace.md#name)
* [onDidChangeConfiguration](_index_d_._plugin_.workspace.md#ondidchangeconfiguration)
* [onDidChangeTextDocument](_index_d_._plugin_.workspace.md#ondidchangetextdocument)
* [onDidChangeWorkspaceFolders](_index_d_._plugin_.workspace.md#ondidchangeworkspacefolders)
* [onDidCloseTextDocument](_index_d_._plugin_.workspace.md#ondidclosetextdocument)
* [onDidCreateFiles](_index_d_._plugin_.workspace.md#ondidcreatefiles)
* [onDidDeleteFiles](_index_d_._plugin_.workspace.md#ondiddeletefiles)
* [onDidOpenTextDocument](_index_d_._plugin_.workspace.md#ondidopentextdocument)
* [onDidRenameFiles](_index_d_._plugin_.workspace.md#ondidrenamefiles)
* [onDidSaveTextDocument](_index_d_._plugin_.workspace.md#ondidsavetextdocument)
* [onWillCreateFiles](_index_d_._plugin_.workspace.md#onwillcreatefiles)
* [onWillDeleteFiles](_index_d_._plugin_.workspace.md#onwilldeletefiles)
* [onWillRenameFiles](_index_d_._plugin_.workspace.md#onwillrenamefiles)
* [onWillSaveTextDocument](_index_d_._plugin_.workspace.md#onwillsavetextdocument)
* [rootPath](_index_d_._plugin_.workspace.md#rootpath)
* [textDocuments](_index_d_._plugin_.workspace.md#textdocuments)
* [workspaceFile](_index_d_._plugin_.workspace.md#workspacefile)
* [workspaceFolders](_index_d_._plugin_.workspace.md#workspacefolders)

### Functions

* [applyEdit](_index_d_._plugin_.workspace.md#applyedit)
* [asRelativePath](_index_d_._plugin_.workspace.md#asrelativepath)
* [createFileSystemWatcher](_index_d_._plugin_.workspace.md#createfilesystemwatcher)
* [findFiles](_index_d_._plugin_.workspace.md#findfiles)
* [getConfiguration](_index_d_._plugin_.workspace.md#getconfiguration)
* [getWorkspaceFolder](_index_d_._plugin_.workspace.md#getworkspacefolder)
* [openTextDocument](_index_d_._plugin_.workspace.md#opentextdocument)
* [registerFileSystemProvider](_index_d_._plugin_.workspace.md#registerfilesystemprovider)
* [registerTaskProvider](_index_d_._plugin_.workspace.md#registertaskprovider)
* [registerTextDocumentContentProvider](_index_d_._plugin_.workspace.md#registertextdocumentcontentprovider)
* [saveAll](_index_d_._plugin_.workspace.md#saveall)
* [updateWorkspaceFolders](_index_d_._plugin_.workspace.md#updateworkspacefolders)

## Variables

### fs

• `Const` **fs**: [FileSystem](../interfaces/_index_d_._plugin_.filesystem.md)

*Defined in [index.d.ts:8946](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8946)*

A [file system](#FileSystem) instance that allows to interact with local and remote
files, e.g. `vscode.workspace.fs.readDirectory(someUri)` allows to retrieve all entries
of a directory or `vscode.workspace.fs.stat(anotherUri)` returns the meta data for a
file.

___

### name

• `Const` **name**: string \| undefined

*Defined in [index.d.ts:8966](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8966)*

The name of the workspace. `undefined` when no folder
has been opened.

___

### onDidChangeConfiguration

• `Const` **onDidChangeConfiguration**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[ConfigurationChangeEvent](../interfaces/_index_d_._plugin_.configurationchangeevent.md)>

*Defined in [index.d.ts:9325](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9325)*

An event that is emitted when the [configuration](#WorkspaceConfiguration) changed.

___

### onDidChangeTextDocument

• `Const` **onDidChangeTextDocument**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[TextDocumentChangeEvent](../interfaces/_index_d_._plugin_.textdocumentchangeevent.md)>

*Defined in [index.d.ts:9215](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9215)*

An event that is emitted when a [text document](#TextDocument) is changed. This usually happens
when the [contents](#TextDocument.getText) changes but also when other things like the
[dirty](#TextDocument.isDirty)-state changes.

___

### onDidChangeWorkspaceFolders

• `Const` **onDidChangeWorkspaceFolders**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[WorkspaceFoldersChangeEvent](../interfaces/_index_d_._plugin_.workspacefolderschangeevent.md)>

*Defined in [index.d.ts:9002](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9002)*

An event that is emitted when a workspace folder is added or removed.

___

### onDidCloseTextDocument

• `Const` **onDidCloseTextDocument**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[TextDocument](../interfaces/_index_d_._plugin_.textdocument.md)>

*Defined in [index.d.ts:9208](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9208)*

An event that is emitted when a [text document](#TextDocument) is disposed or when the language id
of a text document [has been changed](#languages.setTextDocumentLanguage).

To add an event listener when a visible text document is closed, use the [TextEditor](#TextEditor) events in the
[window](#window) namespace. Note that this event is not emitted when a [TextEditor](#TextEditor) is closed
but the document remains open in another [visible text editor](#window.visibleTextEditors).

___

### onDidCreateFiles

• `Const` **onDidCreateFiles**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[FileCreateEvent](../interfaces/_index_d_._plugin_.filecreateevent.md)>

*Defined in [index.d.ts:9257](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9257)*

An event that is emitted when files have been created.

*Note:* This event is triggered by user gestures, like creating a file from the
explorer, or from the [`workspace.applyEdit`](#workspace.applyEdit)-api, but this event is *not* fired when
files change on disk, e.g triggered by another application, or when using the
[`workspace.fs`](#FileSystem)-api.

___

### onDidDeleteFiles

• `Const` **onDidDeleteFiles**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[FileDeleteEvent](../interfaces/_index_d_._plugin_.filedeleteevent.md)>

*Defined in [index.d.ts:9281](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9281)*

An event that is emitted when files have been deleted.

*Note 1:* This event is triggered by user gestures, like deleting a file from the
explorer, or from the [`workspace.applyEdit`](#workspace.applyEdit)-api, but this event is *not* fired when
files change on disk, e.g triggered by another application, or when using the
[`workspace.fs`](#FileSystem)-api.

*Note 2:* When deleting a folder with children only one event is fired.

___

### onDidOpenTextDocument

• `Const` **onDidOpenTextDocument**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[TextDocument](../interfaces/_index_d_._plugin_.textdocument.md)>

*Defined in [index.d.ts:9198](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9198)*

An event that is emitted when a [text document](#TextDocument) is opened or when the language id
of a text document [has been changed](#languages.setTextDocumentLanguage).

To add an event listener when a visible text document is opened, use the [TextEditor](#TextEditor) events in the
[window](#window) namespace. Note that:

- The event is emitted before the [document](#TextDocument) is updated in the
[active text editor](#window.activeTextEditor)
- When a [text document](#TextDocument) is already open (e.g.: open in another [visible text editor](#window.visibleTextEditors)) this event is not emitted

___

### onDidRenameFiles

• `Const` **onDidRenameFiles**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[FileRenameEvent](../interfaces/_index_d_._plugin_.filerenameevent.md)>

*Defined in [index.d.ts:9305](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9305)*

An event that is emitted when files have been renamed.

*Note 1:* This event is triggered by user gestures, like renaming a file from the
explorer, and from the [`workspace.applyEdit`](#workspace.applyEdit)-api, but this event is *not* fired when
files change on disk, e.g triggered by another application, or when using the
[`workspace.fs`](#FileSystem)-api.

*Note 2:* When renaming a folder with children only one event is fired.

___

### onDidSaveTextDocument

• `Const` **onDidSaveTextDocument**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[TextDocument](../interfaces/_index_d_._plugin_.textdocument.md)>

*Defined in [index.d.ts:9235](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9235)*

An event that is emitted when a [text document](#TextDocument) is saved to disk.

___

### onWillCreateFiles

• `Const` **onWillCreateFiles**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[FileWillCreateEvent](../interfaces/_index_d_._plugin_.filewillcreateevent.md)>

*Defined in [index.d.ts:9247](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9247)*

An event that is emitted when files are being created.

*Note 1:* This event is triggered by user gestures, like creating a file from the
explorer, or from the [`workspace.applyEdit`](#workspace.applyEdit)-api. This event is *not* fired when
files change on disk, e.g triggered by another application, or when using the
[`workspace.fs`](#FileSystem)-api.

*Note 2:* When this event is fired, edits to files thare are being created cannot be applied.

___

### onWillDeleteFiles

• `Const` **onWillDeleteFiles**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[FileWillDeleteEvent](../interfaces/_index_d_._plugin_.filewilldeleteevent.md)>

*Defined in [index.d.ts:9269](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9269)*

An event that is emitted when files are being deleted.

*Note 1:* This event is triggered by user gestures, like deleting a file from the
explorer, or from the [`workspace.applyEdit`](#workspace.applyEdit)-api, but this event is *not* fired when
files change on disk, e.g triggered by another application, or when using the
[`workspace.fs`](#FileSystem)-api.

*Note 2:* When deleting a folder with children only one event is fired.

___

### onWillRenameFiles

• `Const` **onWillRenameFiles**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[FileWillRenameEvent](../interfaces/_index_d_._plugin_.filewillrenameevent.md)>

*Defined in [index.d.ts:9293](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9293)*

An event that is emitted when files are being renamed.

*Note 1:* This event is triggered by user gestures, like renaming a file from the
explorer, and from the [`workspace.applyEdit`](#workspace.applyEdit)-api, but this event is *not* fired when
files change on disk, e.g triggered by another application, or when using the
[`workspace.fs`](#FileSystem)-api.

*Note 2:* When renaming a folder with children only one event is fired.

___

### onWillSaveTextDocument

• `Const` **onWillSaveTextDocument**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[TextDocumentWillSaveEvent](../interfaces/_index_d_._plugin_.textdocumentwillsaveevent.md)>

*Defined in [index.d.ts:9230](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9230)*

An event that is emitted when a [text document](#TextDocument) will be saved to disk.

*Note 1:* Subscribers can delay saving by registering asynchronous work. For the sake of data integrity the editor
might save without firing this event. For instance when shutting down with dirty files.

*Note 2:* Subscribers are called sequentially and they can [delay](#TextDocumentWillSaveEvent.waitUntil) saving
by registering asynchronous work. Protection against misbehaving listeners is implemented as such:
 * there is an overall time budget that all listeners share and if that is exhausted no further listener is called
 * listeners that take a long time or produce errors frequently will not be called anymore

The current thresholds are 1.5 seconds as overall time budget and a listener can misbehave 3 times before being ignored.

___

### rootPath

• `Const` **rootPath**: string \| undefined

*Defined in [index.d.ts:8954](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8954)*

~~The folder that is open in the editor. `undefined` when no folder
has been opened.~~

**`deprecated`** Use [`workspaceFolders`](#workspace.workspaceFolders) instead.

___

### textDocuments

• `Const` **textDocuments**: ReadonlyArray\<[TextDocument](../interfaces/_index_d_._plugin_.textdocument.md)>

*Defined in [index.d.ts:9134](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9134)*

All text documents currently known to the system.

___

### workspaceFile

• `Const` **workspaceFile**: [Uri](../classes/_index_d_._plugin_.uri.md) \| undefined

*Defined in [index.d.ts:8997](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8997)*

The location of the workspace file, for example:

`file:///Users/name/Development/myProject.code-workspace`

or

`untitled:1555503116870`

for a workspace that is untitled and not yet saved.

Depending on the workspace that is opened, the value will be:
 * `undefined` when no workspace or  a single folder is opened
 * the path of the workspace file as `Uri` otherwise. if the workspace
is untitled, the returned URI will use the `untitled:` scheme

The location can e.g. be used with the `vscode.openFolder` command to
open the workspace again after it has been closed.

**Example:**
```typescript
vscode.commands.executeCommand('vscode.openFolder', uriOfWorkspace);
```

**Note:** it is not advised to use `workspace.workspaceFile` to write
configuration data into the file. You can use `workspace.getConfiguration().update()`
for that purpose which will work both when a single folder is opened as
well as an untitled or saved workspace.

___

### workspaceFolders

• `Const` **workspaceFolders**: ReadonlyArray\<[WorkspaceFolder](../interfaces/_index_d_._plugin_.workspacefolder.md)> \| undefined

*Defined in [index.d.ts:8960](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8960)*

List of workspace folders or `undefined` when no folder is open.
*Note* that the first entry corresponds to the value of `rootPath`.

## Functions

### applyEdit

▸ **applyEdit**(`edit`: [WorkspaceEdit](../classes/_index_d_._plugin_.workspaceedit.md)): [Thenable](../interfaces/_index_d_.thenable.md)\<boolean>

*Defined in [index.d.ts:9129](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9129)*

Make changes to one or many resources or create, delete, and rename resources as defined by the given
[workspace edit](#WorkspaceEdit).

All changes of a workspace edit are applied in the same order in which they have been added. If
multiple textual inserts are made at the same position, these strings appear in the resulting text
in the order the 'inserts' were made, unless that are interleaved with resource edits. Invalid sequences
like 'delete file a' -> 'insert text in file a' cause failure of the operation.

When applying a workspace edit that consists only of text edits an 'all-or-nothing'-strategy is used.
A workspace edit with resource creations or deletions aborts the operation, e.g. consecutive edits will
not be attempted, when a single edit fails.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`edit` | [WorkspaceEdit](../classes/_index_d_._plugin_.workspaceedit.md) | A workspace edit. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<boolean>

A thenable that resolves when the edit could be applied.

___

### asRelativePath

▸ **asRelativePath**(`pathOrUri`: string \| [Uri](../classes/_index_d_._plugin_.uri.md), `includeWorkspaceFolder?`: boolean): string

*Defined in [index.d.ts:9026](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9026)*

Returns a path that is relative to the workspace folder or folders.

When there are no [workspace folders](#workspace.workspaceFolders) or when the path
is not contained in them, the input is returned.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`pathOrUri` | string \| [Uri](../classes/_index_d_._plugin_.uri.md) | A path or uri. When a uri is given its [fsPath](#Uri.fsPath) is used. |
`includeWorkspaceFolder?` | boolean | When `true` and when the given path is contained inside a workspace folder the name of the workspace is prepended. Defaults to `true` when there are multiple workspace folders and `false` otherwise. |

**Returns:** string

A path relative to the root or the input.

___

### createFileSystemWatcher

▸ **createFileSystemWatcher**(`globPattern`: [GlobPattern](_index_d_._plugin_.md#globpattern), `ignoreCreateEvents?`: boolean, `ignoreChangeEvents?`: boolean, `ignoreDeleteEvents?`: boolean): [FileSystemWatcher](../interfaces/_index_d_._plugin_.filesystemwatcher.md)

*Defined in [index.d.ts:9086](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9086)*

Creates a file system watcher.

A glob pattern that filters the file events on their absolute path must be provided. Optionally,
flags to ignore certain kinds of events can be provided. To stop listening to events the watcher must be disposed.

*Note* that only files within the current [workspace folders](#workspace.workspaceFolders) can be watched.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`globPattern` | [GlobPattern](_index_d_._plugin_.md#globpattern) | A [glob pattern](#GlobPattern) that is applied to the absolute paths of created, changed, and deleted files. Use a [relative pattern](#RelativePattern) to limit events to a certain [workspace folder](#WorkspaceFolder). |
`ignoreCreateEvents?` | boolean | Ignore when files have been created. |
`ignoreChangeEvents?` | boolean | Ignore when files have been changed. |
`ignoreDeleteEvents?` | boolean | Ignore when files have been deleted. |

**Returns:** [FileSystemWatcher](../interfaces/_index_d_._plugin_.filesystemwatcher.md)

A new file system watcher instance.

___

### findFiles

▸ **findFiles**(`include`: [GlobPattern](_index_d_._plugin_.md#globpattern), `exclude?`: [GlobPattern](_index_d_._plugin_.md#globpattern) \| null, `maxResults?`: number, `token?`: [CancellationToken](../interfaces/_index_d_._plugin_.cancellationtoken.md)): [Thenable](../interfaces/_index_d_.thenable.md)\<[Uri](../classes/_index_d_._plugin_.uri.md)[]>

*Defined in [index.d.ts:9103](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9103)*

Find files across all [workspace folders](#workspace.workspaceFolders) in the workspace.

**`sample`** `findFiles('**​/*.js', '**​/node_modules/**', 10)`

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`include` | [GlobPattern](_index_d_._plugin_.md#globpattern) | A [glob pattern](#GlobPattern) that defines the files to search for. The glob pattern will be matched against the file paths of resulting matches relative to their workspace. Use a [relative pattern](#RelativePattern) to restrict the search results to a [workspace folder](#WorkspaceFolder). |
`exclude?` | [GlobPattern](_index_d_._plugin_.md#globpattern) \| null | A [glob pattern](#GlobPattern) that defines files and folders to exclude. The glob pattern will be matched against the file paths of resulting matches relative to their workspace. When `undefined` only default excludes will apply, when `null` no excludes will apply. |
`maxResults?` | number | An upper-bound for the result. |
`token?` | [CancellationToken](../interfaces/_index_d_._plugin_.cancellationtoken.md) | A token that can be used to signal cancellation to the underlying search engine. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<[Uri](../classes/_index_d_._plugin_.uri.md)[]>

A thenable that resolves to an array of resource identifiers. Will return no results if no
[workspace folders](#workspace.workspaceFolders) are opened.

___

### getConfiguration

▸ **getConfiguration**(`section?`: string \| undefined, `scope?`: [ConfigurationScope](_index_d_._plugin_.md#configurationscope) \| null): [WorkspaceConfiguration](../interfaces/_index_d_._plugin_.workspaceconfiguration.md)

*Defined in [index.d.ts:9320](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9320)*

Get a workspace configuration object.

When a section-identifier is provided only that part of the configuration
is returned. Dots in the section-identifier are interpreted as child-access,
like `{ myExt: { setting: { doIt: true }}}` and `getConfiguration('myExt.setting').get('doIt') === true`.

When a scope is provided configuraiton confined to that scope is returned. Scope can be a resource or a language identifier or both.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`section?` | string \| undefined | A dot-separated identifier. |
`scope?` | [ConfigurationScope](_index_d_._plugin_.md#configurationscope) \| null | A scope for which the configuration is asked for. |

**Returns:** [WorkspaceConfiguration](../interfaces/_index_d_._plugin_.workspaceconfiguration.md)

The full configuration or a subset.

___

### getWorkspaceFolder

▸ **getWorkspaceFolder**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md)): [WorkspaceFolder](../interfaces/_index_d_._plugin_.workspacefolder.md) \| undefined

*Defined in [index.d.ts:9012](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9012)*

Returns the [workspace folder](#WorkspaceFolder) that contains a given uri.
* returns `undefined` when the given uri doesn't match any workspace folder
* returns the *input* when the given uri is a workspace folder itself

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | An uri. |

**Returns:** [WorkspaceFolder](../interfaces/_index_d_._plugin_.workspacefolder.md) \| undefined

A workspace folder or `undefined`

___

### openTextDocument

▸ **openTextDocument**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md)): [Thenable](../interfaces/_index_d_.thenable.md)\<[TextDocument](../interfaces/_index_d_._plugin_.textdocument.md)>

*Defined in [index.d.ts:9154](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9154)*

Opens a document. Will return early if this document is already open. Otherwise
the document is loaded and the [didOpen](#workspace.onDidOpenTextDocument)-event fires.

The document is denoted by an [uri](#Uri). Depending on the [scheme](#Uri.scheme) the
following rules apply:
* `file`-scheme: Open a file on disk, will be rejected if the file does not exist or cannot be loaded.
* `untitled`-scheme: A new file that should be saved on disk, e.g. `untitled:c:\frodo\new.js`. The language
will be derived from the file name.
* For all other schemes contributed [text document content providers](#TextDocumentContentProvider) and
[file system providers](#FileSystemProvider) are consulted.

*Note* that the lifecycle of the returned document is owned by the editor and not by the extension. That means an
[`onDidClose`](#workspace.onDidCloseTextDocument)-event can occur at any time after opening it.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | Identifies the resource to open. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<[TextDocument](../interfaces/_index_d_._plugin_.textdocument.md)>

A promise that resolves to a [document](#TextDocument).

▸ **openTextDocument**(`fileName`: string): [Thenable](../interfaces/_index_d_.thenable.md)\<[TextDocument](../interfaces/_index_d_._plugin_.textdocument.md)>

*Defined in [index.d.ts:9163](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9163)*

A short-hand for `openTextDocument(Uri.file(fileName))`.

**`see`** [openTextDocument](#openTextDocument)

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`fileName` | string | A name of a file on disk. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<[TextDocument](../interfaces/_index_d_._plugin_.textdocument.md)>

A promise that resolves to a [document](#TextDocument).

▸ **openTextDocument**(`options?`: { content?: string ; language?: string  }): [Thenable](../interfaces/_index_d_.thenable.md)\<[TextDocument](../interfaces/_index_d_._plugin_.textdocument.md)>

*Defined in [index.d.ts:9173](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9173)*

Opens an untitled text document. The editor will prompt the user for a file
path when the document is to be saved. The `options` parameter allows to
specify the *language* and/or the *content* of the document.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`options?` | { content?: string ; language?: string  } | Options to control how the document will be created. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<[TextDocument](../interfaces/_index_d_._plugin_.textdocument.md)>

A promise that resolves to a [document](#TextDocument).

___

### registerFileSystemProvider

▸ **registerFileSystemProvider**(`scheme`: string, `provider`: [FileSystemProvider](../interfaces/_index_d_._plugin_.filesystemprovider.md), `options?`: { isCaseSensitive?: boolean ; isReadonly?: boolean  }): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:9349](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9349)*

Register a filesystem provider for a given scheme, e.g. `ftp`.

There can only be one provider per scheme and an error is being thrown when a scheme
has been claimed by another provider or when it is reserved.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`scheme` | string | The uri-[scheme](#Uri.scheme) the provider registers for. |
`provider` | [FileSystemProvider](../interfaces/_index_d_._plugin_.filesystemprovider.md) | The filesystem provider. |
`options?` | { isCaseSensitive?: boolean ; isReadonly?: boolean  } | Immutable metadata about the provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerTaskProvider

▸ **registerTaskProvider**(`type`: string, `provider`: [TaskProvider](../interfaces/_index_d_._plugin_.taskprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:9336](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9336)*

~~Register a task provider.~~

**`deprecated`** Use the corresponding function on the `tasks` namespace instead

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`type` | string | The task kind type this provider is registered for. |
`provider` | [TaskProvider](../interfaces/_index_d_._plugin_.taskprovider.md) | A task provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerTextDocumentContentProvider

▸ **registerTextDocumentContentProvider**(`scheme`: string, `provider`: [TextDocumentContentProvider](../interfaces/_index_d_._plugin_.textdocumentcontentprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:9184](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9184)*

Register a text document content provider.

Only one provider can be registered per scheme.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`scheme` | string | The uri-scheme to register for. |
`provider` | [TextDocumentContentProvider](../interfaces/_index_d_._plugin_.textdocumentcontentprovider.md) | A content provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### saveAll

▸ **saveAll**(`includeUntitled?`: boolean): [Thenable](../interfaces/_index_d_.thenable.md)\<boolean>

*Defined in [index.d.ts:9111](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9111)*

Save all dirty files.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`includeUntitled?` | boolean | Also save files that have been created during this session. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<boolean>

A thenable that resolves when the files have been saved.

___

### updateWorkspaceFolders

▸ **updateWorkspaceFolders**(`start`: number, `deleteCount`: number \| undefined \| null, ...`workspaceFoldersToAdd`: { name?: string ; uri: [Uri](../classes/_index_d_._plugin_.uri.md)  }[]): boolean

*Defined in [index.d.ts:9069](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9069)*

This method replaces `deleteCount` [workspace folders](#workspace.workspaceFolders) starting at index `start`
by an optional set of `workspaceFoldersToAdd` on the `vscode.workspace.workspaceFolders` array. This "splice"
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

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`start` | number | the zero-based location in the list of currently opened [workspace folders](#WorkspaceFolder) from which to start deleting workspace folders. |
`deleteCount` | number \| undefined \| null | the optional number of workspace folders to remove. |
`...workspaceFoldersToAdd` | { name?: string ; uri: [Uri](../classes/_index_d_._plugin_.uri.md)  }[] | the optional variable set of workspace folders to add in place of the deleted ones. Each workspace is identified with a mandatory URI and an optional name. |

**Returns:** boolean

true if the operation was successfully started and false otherwise if arguments were used that would result
in invalid workspace folder state (e.g. 2 folders with the same URI).
