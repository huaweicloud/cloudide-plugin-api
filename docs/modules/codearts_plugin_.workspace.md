[@codearts/plugin](../README.md) / ["@codearts/plugin"](_codearts_plugin_.md) / workspace

# Namespace: workspace

["@codearts/plugin"](_codearts_plugin_.md).workspace

Namespace for dealing with the current workspace. A workspace is the collection of one
or more folders that are opened in an editor window (instance).

It is also possible to open an editor without a workspace. For example, when you open a
new editor window by selecting a file from your platform's File menu, you will not be
inside a workspace. In this mode, some of the editor's capabilities are reduced but you can
still open text files and edit them.

Refer to https://code.visualstudio.com/docs/editor/workspaces for more information on
the concept of workspaces.

The workspace offers support for [listening](codearts_plugin_.workspace.md#createfilesystemwatcher) to fs
events and for [finding](codearts_plugin_.workspace.md#findfiles) files. Both perform well and run _outside_
the editor-process so that they should be always used instead of nodejs-equivalents.

## Table of contents

### Interfaces

- [ConfigurationPropertySchema](../interfaces/codearts_plugin_.workspace.ConfigurationPropertySchema.md)
- [JSONSchema](../interfaces/codearts_plugin_.workspace.JSONSchema.md)
- [JSONSchemaMap](../interfaces/codearts_plugin_.workspace.JSONSchemaMap.md)
- [JSONSchemaSnippet](../interfaces/codearts_plugin_.workspace.JSONSchemaSnippet.md)
- [Policy](../interfaces/codearts_plugin_.workspace.Policy.md)

### Type Aliases

- [JSONSchemaType](codearts_plugin_.workspace.md#jsonschematype)

### Variables

- [fs](codearts_plugin_.workspace.md#fs)
- [isTrusted](codearts_plugin_.workspace.md#istrusted)
- [name](codearts_plugin_.workspace.md#name)
- [notebookDocuments](codearts_plugin_.workspace.md#notebookdocuments)
- [rootPath](codearts_plugin_.workspace.md#rootpath)
- [textDocuments](codearts_plugin_.workspace.md#textdocuments)
- [workspaceFile](codearts_plugin_.workspace.md#workspacefile)
- [workspaceFolders](codearts_plugin_.workspace.md#workspacefolders)

### Functions

- [applyEdit](codearts_plugin_.workspace.md#applyedit)
- [asRelativePath](codearts_plugin_.workspace.md#asrelativepath)
- [createFileSystemWatcher](codearts_plugin_.workspace.md#createfilesystemwatcher)
- [findFiles](codearts_plugin_.workspace.md#findfiles)
- [getConfiguration](codearts_plugin_.workspace.md#getconfiguration)
- [getWorkspaceFolder](codearts_plugin_.workspace.md#getworkspacefolder)
- [onDidChangeConfiguration](codearts_plugin_.workspace.md#ondidchangeconfiguration)
- [onDidChangeNotebookDocument](codearts_plugin_.workspace.md#ondidchangenotebookdocument)
- [onDidChangeTextDocument](codearts_plugin_.workspace.md#ondidchangetextdocument)
- [onDidChangeWorkspaceFolders](codearts_plugin_.workspace.md#ondidchangeworkspacefolders)
- [onDidCloseNotebookDocument](codearts_plugin_.workspace.md#ondidclosenotebookdocument)
- [onDidCloseTextDocument](codearts_plugin_.workspace.md#ondidclosetextdocument)
- [onDidCreateFiles](codearts_plugin_.workspace.md#ondidcreatefiles)
- [onDidDeleteFiles](codearts_plugin_.workspace.md#ondiddeletefiles)
- [onDidGrantWorkspaceTrust](codearts_plugin_.workspace.md#ondidgrantworkspacetrust)
- [onDidOpenNotebookDocument](codearts_plugin_.workspace.md#ondidopennotebookdocument)
- [onDidOpenTextDocument](codearts_plugin_.workspace.md#ondidopentextdocument)
- [onDidRenameFiles](codearts_plugin_.workspace.md#ondidrenamefiles)
- [onDidSaveNotebookDocument](codearts_plugin_.workspace.md#ondidsavenotebookdocument)
- [onDidSaveTextDocument](codearts_plugin_.workspace.md#ondidsavetextdocument)
- [onWillCreateFiles](codearts_plugin_.workspace.md#onwillcreatefiles)
- [onWillDeleteFiles](codearts_plugin_.workspace.md#onwilldeletefiles)
- [onWillRenameFiles](codearts_plugin_.workspace.md#onwillrenamefiles)
- [onWillSaveTextDocument](codearts_plugin_.workspace.md#onwillsavetextdocument)
- [openNotebookDocument](codearts_plugin_.workspace.md#opennotebookdocument)
- [openTextDocument](codearts_plugin_.workspace.md#opentextdocument)
- [registerConfiguration](codearts_plugin_.workspace.md#registerconfiguration)
- [registerFileSystemProvider](codearts_plugin_.workspace.md#registerfilesystemprovider)
- [registerNotebookSerializer](codearts_plugin_.workspace.md#registernotebookserializer)
- [registerTaskProvider](codearts_plugin_.workspace.md#registertaskprovider)
- [registerTextDocumentContentProvider](codearts_plugin_.workspace.md#registertextdocumentcontentprovider)
- [saveAll](codearts_plugin_.workspace.md#saveall)
- [updateConfigurationOption](codearts_plugin_.workspace.md#updateconfigurationoption)
- [updateWorkspaceFolders](codearts_plugin_.workspace.md#updateworkspacefolders)

## Type Aliases

### JSONSchemaType

Ƭ **JSONSchemaType**: ``"string"`` \| ``"number"`` \| ``"integer"`` \| ``"boolean"`` \| ``"null"`` \| ``"array"`` \| ``"object"``

Type in JSONSchema

#### Defined in

[index.d.ts:12920](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12920)

## Variables

### fs

• `Const` **fs**: [`FileSystem`](../interfaces/codearts_plugin_.FileSystem.md)

A [file system](../interfaces/codearts_plugin_.FileSystem.md) instance that allows to interact with local and remote
files, e.g. `vscode.workspace.fs.readDirectory(someUri)` allows to retrieve all entries
of a directory or `vscode.workspace.fs.stat(anotherUri)` returns the meta data for a
file.

#### Defined in

[index.d.ts:12112](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12112)

___

### isTrusted

• `Const` **isTrusted**: `boolean`

When true, the user has explicitly trusted the contents of the workspace.

#### Defined in

[index.d.ts:12978](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12978)

___

### name

• `Const` **name**: `string` \| `undefined`

The name of the workspace. `undefined` when no workspace
has been opened.

Refer to https://code.visualstudio.com/docs/editor/workspaces for more information on
the concept of workspaces.

#### Defined in

[index.d.ts:12141](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12141)

___

### notebookDocuments

• `Const` **notebookDocuments**: readonly [`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md)[]

All notebook documents currently known to the editor.

#### Defined in

[index.d.ts:12535](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12535)

___

### rootPath

• `Const` **rootPath**: `string` \| `undefined`

The uri of the first entry of [`workspaceFolders`](codearts_plugin_.workspace.md#workspacefolders)
as `string`. `undefined` if there is no first entry.

Refer to https://code.visualstudio.com/docs/editor/workspaces for more information
on workspaces.

**`Deprecated`**

Use [`workspaceFolders`](codearts_plugin_.workspace.md#workspacefolders) instead.

#### Defined in

[index.d.ts:12123](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12123)

___

### textDocuments

• `Const` **textDocuments**: readonly [`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)[]

All text documents currently known to the editor.

#### Defined in

[index.d.ts:12426](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12426)

___

### workspaceFile

• `Const` **workspaceFile**: [`Uri`](../classes/codearts_plugin_.Uri.md) \| `undefined`

The location of the workspace file, for example:

`file:///Users/name/Development/myProject.code-workspace`

or

`untitled:1555503116870`

for a workspace that is untitled and not yet saved.

Depending on the workspace that is opened, the value will be:
 * `undefined` when no workspace is opened
 * the path of the workspace file as `Uri` otherwise. if the workspace
is untitled, the returned URI will use the `untitled:` scheme

The location can e.g. be used with the `vscode.openFolder` command to
open the workspace again after it has been closed.

**Example:**
```typescript
vscode.commands.executeCommand('vscode.openFolder', uriOfWorkspace);
```

Refer to https://code.visualstudio.com/docs/editor/workspaces for more information on
the concept of workspaces.

**Note:** it is not advised to use `workspace.workspaceFile` to write
configuration data into the file. You can use `workspace.getConfiguration().update()`
for that purpose which will work both when a single folder is opened as
well as an untitled or saved workspace.

#### Defined in

[index.d.ts:12175](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12175)

___

### workspaceFolders

• `Const` **workspaceFolders**: readonly [`WorkspaceFolder`](../interfaces/codearts_plugin_.WorkspaceFolder.md)[] \| `undefined`

List of workspace folders (0-N) that are open in the editor. `undefined` when no workspace
has been opened.

Refer to https://code.visualstudio.com/docs/editor/workspaces for more information
on workspaces.

#### Defined in

[index.d.ts:12132](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12132)

## Functions

### applyEdit

▸ **applyEdit**(`edit`): [`Thenable`](../interfaces/Thenable.md)<`boolean`\>

Make changes to one or many resources or create, delete, and rename resources as defined by the given
[workspace edit](../classes/codearts_plugin_.WorkspaceEdit.md).

All changes of a workspace edit are applied in the same order in which they have been added. If
multiple textual inserts are made at the same position, these strings appear in the resulting text
in the order the 'inserts' were made, unless that are interleaved with resource edits. Invalid sequences
like 'delete file a' -> 'insert text in file a' cause failure of the operation.

When applying a workspace edit that consists only of text edits an 'all-or-nothing'-strategy is used.
A workspace edit with resource creations or deletions aborts the operation, e.g. consecutive edits will
not be attempted, when a single edit fails.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `edit` | [`WorkspaceEdit`](../classes/codearts_plugin_.WorkspaceEdit.md) | A workspace edit. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`boolean`\>

A thenable that resolves when the edit could be applied.

#### Defined in

[index.d.ts:12421](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12421)

___

### asRelativePath

▸ **asRelativePath**(`pathOrUri`, `includeWorkspaceFolder?`): `string`

Returns a path that is relative to the workspace folder or folders.

When there are no [workspace folders](codearts_plugin_.workspace.md#workspacefolders) or when the path
is not contained in them, the input is returned.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pathOrUri` | `string` \| [`Uri`](../classes/codearts_plugin_.Uri.md) | A path or uri. When a uri is given its [fsPath](../classes/codearts_plugin_.Uri.md#fspath) is used. |
| `includeWorkspaceFolder?` | `boolean` | When `true` and when the given path is contained inside a workspace folder the name of the workspace is prepended. Defaults to `true` when there are multiple workspace folders and `false` otherwise. |

#### Returns

`string`

A path relative to the root or the input.

#### Defined in

[index.d.ts:12209](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12209)

___

### createFileSystemWatcher

▸ **createFileSystemWatcher**(`globPattern`, `ignoreCreateEvents?`, `ignoreChangeEvents?`, `ignoreDeleteEvents?`): [`FileSystemWatcher`](../interfaces/codearts_plugin_.FileSystemWatcher.md)

Creates a file system watcher that is notified on file events (create, change, delete)
depending on the parameters provided.

By default, all opened [workspace folders](codearts_plugin_.workspace.md#workspacefolders) will be watched
for file changes recursively.

Additional paths can be added for file watching by providing a [RelativePattern](../classes/codearts_plugin_.RelativePattern.md) with
a `base` path to watch. If the `pattern` is complex (e.g. contains `**` or path segments),
the path will be watched recursively and otherwise will be watched non-recursively (i.e. only
changes to the first level of the path will be reported).

*Note* that requests for recursive file watchers for a `base` path that is inside the opened
workspace are ignored given all opened [workspace folders](codearts_plugin_.workspace.md#workspacefolders) are
watched for file changes recursively by default. Non-recursive file watchers however are always
supported, even inside the opened workspace because they allow to bypass the configured settings
for excludes (`files.watcherExclude`). If you need to watch in a location that is typically
excluded (for example `node_modules` or `.git` folder), then you can use a non-recursive watcher
in the workspace for this purpose.

If possible, keep the use of recursive watchers to a minimum because recursive file watching
is quite resource intense.

Providing a `string` as `globPattern` acts as convenience method for watching file events in
all opened workspace folders. It cannot be used to add more folders for file watching, nor will
it report any file events from folders that are not part of the opened workspace folders.

Optionally, flags to ignore certain kinds of events can be provided.

To stop listening to events the watcher must be disposed.

*Note* that file events from recursive file watchers may be excluded based on user configuration.
The setting `files.watcherExclude` helps to reduce the overhead of file events from folders
that are known to produce many file changes at once (such as `node_modules` folders). As such,
it is highly recommended to watch with simple patterns that do not require recursive watchers
where the exclude settings are ignored and you have full control over the events.

*Note* that symbolic links are not automatically followed for file watching unless the path to
watch itself is a symbolic link.

*Note* that file changes for the path to be watched may not be delivered when the path itself
changes. For example, when watching a path `/Users/somename/Desktop` and the path itself is
being deleted, the watcher may not report an event and may not work anymore from that moment on.
The underlying behaviour depends on the path that is provided for watching:
* if the path is within any of the workspace folders, deletions are tracked and reported unless
  excluded via `files.watcherExclude` setting
* if the path is equal to any of the workspace folders, deletions are not tracked
* if the path is outside of any of the workspace folders, deletions are not tracked

If you are interested in being notified when the watched path itself is being deleted, you have
to watch it's parent folder. Make sure to use a simple `pattern` (such as putting the name of the
folder) to not accidentally watch all sibling folders recursively.

*Note* that the file paths that are reported for having changed may have a different path casing
compared to the actual casing on disk on case-insensitive platforms (typically macOS and Windows
but not Linux). We allow a user to open a workspace folder with any desired path casing and try
to preserve that. This means:
* if the path is within any of the workspace folders, the path will match the casing of the
  workspace folder up to that portion of the path and match the casing on disk for children
* if the path is outside of any of the workspace folders, the casing will match the case of the
  path that was provided for watching
In the same way, symbolic links are preserved, i.e. the file event will report the path of the
symbolic link as it was provided for watching and not the target.

### Examples

The basic anatomy of a file watcher is as follows:

```ts
const watcher = vscode.workspace.createFileSystemWatcher(new vscode.RelativePattern(<folder>, <pattern>));

watcher.onDidChange(uri => { ... }); // listen to files being changed
watcher.onDidCreate(uri => { ... }); // listen to files/folders being created
watcher.onDidDelete(uri => { ... }); // listen to files/folders getting deleted

watcher.dispose(); // dispose after usage
```

#### Workspace file watching

If you only care about file events in a specific workspace folder:

```ts
vscode.workspace.createFileSystemWatcher(new vscode.RelativePattern(vscode.workspace.workspaceFolders[0], '**​/*.js'));
```

If you want to monitor file events across all opened workspace folders:

```ts
vscode.workspace.createFileSystemWatcher('**​/*.js'));
```

*Note:* the array of workspace folders can be empty if no workspace is opened (empty window).

#### Out of workspace file watching

To watch a folder for changes to *.js files outside the workspace (non recursively), pass in a `Uri` to such
a folder:

```ts
vscode.workspace.createFileSystemWatcher(new vscode.RelativePattern(vscode.Uri.file(<path to folder outside workspace>), '*.js'));
```

And use a complex glob pattern to watch recursively:

```ts
vscode.workspace.createFileSystemWatcher(new vscode.RelativePattern(vscode.Uri.file(<path to folder outside workspace>), '**​/*.js'));
```

Here is an example for watching the active editor for file changes:

```ts
vscode.workspace.createFileSystemWatcher(new vscode.RelativePattern(vscode.window.activeTextEditor.document.uri, '*'));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `globPattern` | [`GlobPattern`](_codearts_plugin_.md#globpattern) | A [glob pattern](_codearts_plugin_.md#globpattern) that controls which file events the watcher should report. |
| `ignoreCreateEvents?` | `boolean` | Ignore when files have been created. |
| `ignoreChangeEvents?` | `boolean` | Ignore when files have been changed. |
| `ignoreDeleteEvents?` | `boolean` | Ignore when files have been deleted. |

#### Returns

[`FileSystemWatcher`](../interfaces/codearts_plugin_.FileSystemWatcher.md)

A new file system watcher instance. Must be disposed when no longer needed.

#### Defined in

[index.d.ts:12375](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12375)

___

### findFiles

▸ **findFiles**(`include`, `exclude?`, `maxResults?`, `token?`): [`Thenable`](../interfaces/Thenable.md)<[`Uri`](../classes/codearts_plugin_.Uri.md)[]\>

Find files across all [workspace folders](codearts_plugin_.workspace.md#workspacefolders) in the workspace.

**`Example`**

```ts
findFiles('**​/*.js', '**​/node_modules/**', 10)
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `include` | [`GlobPattern`](_codearts_plugin_.md#globpattern) | A [glob pattern](_codearts_plugin_.md#globpattern) that defines the files to search for. The glob pattern will be matched against the file paths of resulting matches relative to their workspace. Use a [relative pattern](../classes/codearts_plugin_.RelativePattern.md) to restrict the search results to a [workspace folder](../interfaces/codearts_plugin_.WorkspaceFolder.md). |
| `exclude?` | ``null`` \| [`GlobPattern`](_codearts_plugin_.md#globpattern) | A [glob pattern](_codearts_plugin_.md#globpattern) that defines files and folders to exclude. The glob pattern will be matched against the file paths of resulting matches relative to their workspace. When `undefined`, default file-excludes (e.g. the `files.exclude`-setting but not `search.exclude`) will apply. When `null`, no excludes will apply. |
| `maxResults?` | `number` | An upper-bound for the result. |
| `token?` | [`CancellationToken`](../interfaces/codearts_plugin_.CancellationToken.md) | A token that can be used to signal cancellation to the underlying search engine. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`Uri`](../classes/codearts_plugin_.Uri.md)[]\>

A thenable that resolves to an array of resource identifiers. Will return no results if no
[workspace folders](codearts_plugin_.workspace.md#workspacefolders) are opened.

#### Defined in

[index.d.ts:12394](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12394)

___

### getConfiguration

▸ **getConfiguration**(`section?`, `scope?`): [`WorkspaceConfiguration`](../interfaces/codearts_plugin_.WorkspaceConfiguration.md)

Get a workspace configuration object.

When a section-identifier is provided only that part of the configuration
is returned. Dots in the section-identifier are interpreted as child-access,
like `{ myExt: { setting: { doIt: true }}}` and `getConfiguration('myExt.setting').get('doIt') === true`.

When a scope is provided configuration confined to that scope is returned. Scope can be a resource or a language identifier or both.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `section?` | `string` | A dot-separated identifier. |
| `scope?` | ``null`` \| [`ConfigurationScope`](_codearts_plugin_.md#configurationscope) | A scope for which the configuration is asked for. |

#### Returns

[`WorkspaceConfiguration`](../interfaces/codearts_plugin_.WorkspaceConfiguration.md)

The full configuration or a subset.

#### Defined in

[index.d.ts:12936](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12936)

___

### getWorkspaceFolder

▸ **getWorkspaceFolder**(`uri`): [`WorkspaceFolder`](../interfaces/codearts_plugin_.WorkspaceFolder.md) \| `undefined`

Returns the [workspace folder](../interfaces/codearts_plugin_.WorkspaceFolder.md) that contains a given uri.
* returns `undefined` when the given uri doesn't match any workspace folder
* returns the *input* when the given uri is a workspace folder itself

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | An uri. |

#### Returns

[`WorkspaceFolder`](../interfaces/codearts_plugin_.WorkspaceFolder.md) \| `undefined`

A workspace folder or `undefined`

#### Defined in

[index.d.ts:12195](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12195)

___

### onDidChangeConfiguration

▸ **onDidChangeConfiguration**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`ConfigurationChangeEvent`](../interfaces/codearts_plugin_.ConfigurationChangeEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidChangeNotebookDocument

▸ **onDidChangeNotebookDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`NotebookDocumentChangeEvent`](../interfaces/codearts_plugin_.NotebookDocumentChangeEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidChangeTextDocument

▸ **onDidChangeTextDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TextDocumentChangeEvent`](../interfaces/codearts_plugin_.TextDocumentChangeEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidChangeWorkspaceFolders

▸ **onDidChangeWorkspaceFolders**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`WorkspaceFoldersChangeEvent`](../interfaces/codearts_plugin_.WorkspaceFoldersChangeEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidCloseNotebookDocument

▸ **onDidCloseNotebookDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidCloseTextDocument

▸ **onDidCloseTextDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidCreateFiles

▸ **onDidCreateFiles**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`FileCreateEvent`](../interfaces/codearts_plugin_.FileCreateEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidDeleteFiles

▸ **onDidDeleteFiles**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`FileDeleteEvent`](../interfaces/codearts_plugin_.FileDeleteEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidGrantWorkspaceTrust

▸ **onDidGrantWorkspaceTrust**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: `void`) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidOpenNotebookDocument

▸ **onDidOpenNotebookDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidOpenTextDocument

▸ **onDidOpenTextDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidRenameFiles

▸ **onDidRenameFiles**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`FileRenameEvent`](../interfaces/codearts_plugin_.FileRenameEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidSaveNotebookDocument

▸ **onDidSaveNotebookDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidSaveTextDocument

▸ **onDidSaveTextDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onWillCreateFiles

▸ **onWillCreateFiles**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`FileWillCreateEvent`](../interfaces/codearts_plugin_.FileWillCreateEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onWillDeleteFiles

▸ **onWillDeleteFiles**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`FileWillDeleteEvent`](../interfaces/codearts_plugin_.FileWillDeleteEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onWillRenameFiles

▸ **onWillRenameFiles**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`FileWillRenameEvent`](../interfaces/codearts_plugin_.FileWillRenameEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onWillSaveTextDocument

▸ **onWillSaveTextDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TextDocumentWillSaveEvent`](../interfaces/codearts_plugin_.TextDocumentWillSaveEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### openNotebookDocument

▸ **openNotebookDocument**(`uri`): [`Thenable`](../interfaces/Thenable.md)<[`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md)\>

Open a notebook. Will return early if this notebook is already notebook.notebookDocuments loaded. Otherwise
the notebook is loaded and the notebook.onDidOpenNotebookDocument onDidOpenNotebookDocument-event fires.

*Note* that the lifecycle of the returned notebook is owned by the editor and not by the extension. That means an
notebook.onDidCloseNotebookDocument onDidCloseNotebookDocument-event can occur at any time after.

*Note* that opening a notebook does not show a notebook editor. This function only returns a notebook document which
can be shown in a notebook editor but it can also be used for other things.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The resource to open. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md)\>

A promise that resolves to a [notebook](../interfaces/codearts_plugin_.NotebookDocument.md)

#### Defined in

[index.d.ts:12550](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12550)

▸ **openNotebookDocument**(`notebookType`, `content?`): [`Thenable`](../interfaces/Thenable.md)<[`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md)\>

Open an untitled notebook. The editor will prompt the user for a file
path when the document is to be saved.

**`See`**

[openNotebookDocument](codearts_plugin_.workspace.md#opennotebookdocument)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `notebookType` | `string` | The notebook type that should be used. |
| `content?` | [`NotebookData`](../classes/codearts_plugin_.NotebookData.md) | The initial contents of the notebook. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md)\>

A promise that resolves to a [notebook](../interfaces/codearts_plugin_.NotebookDocument.md).

#### Defined in

[index.d.ts:12561](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12561)

___

### openTextDocument

▸ **openTextDocument**(`uri`): [`Thenable`](../interfaces/Thenable.md)<[`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)\>

Opens a document. Will return early if this document is already open. Otherwise
the document is loaded and the [didOpen](codearts_plugin_.workspace.md#ondidopentextdocument)-event fires.

The document is denoted by an [Uri](../classes/codearts_plugin_.Uri.md). Depending on the [scheme](../classes/codearts_plugin_.Uri.md#scheme) the
following rules apply:
* `file`-scheme: Open a file on disk (`openTextDocument(Uri.file(path))`). Will be rejected if the file
does not exist or cannot be loaded.
* `untitled`-scheme: Open a blank untitled file with associated path (`openTextDocument(Uri.file(path).with({ scheme: 'untitled' }))`).
The language will be derived from the file name.
* For all other schemes contributed [text document content providers](../interfaces/codearts_plugin_.TextDocumentContentProvider.md) and
[file system providers](../interfaces/codearts_plugin_.FileSystemProvider.md) are consulted.

*Note* that the lifecycle of the returned document is owned by the editor and not by the extension. That means an
[`onDidClose`](codearts_plugin_.workspace.md#ondidclosetextdocument)-event can occur at any time after opening it.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | Identifies the resource to open. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)\>

A promise that resolves to a [document](../interfaces/codearts_plugin_.TextDocument.md).

#### Defined in

[index.d.ts:12447](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12447)

▸ **openTextDocument**(`fileName`): [`Thenable`](../interfaces/Thenable.md)<[`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)\>

A short-hand for `openTextDocument(Uri.file(fileName))`.

**`See`**

[openTextDocument](codearts_plugin_.workspace.md#opentextdocument)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fileName` | `string` | A name of a file on disk. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)\>

A promise that resolves to a [document](../interfaces/codearts_plugin_.TextDocument.md).

#### Defined in

[index.d.ts:12456](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12456)

▸ **openTextDocument**(`options?`): [`Thenable`](../interfaces/Thenable.md)<[`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)\>

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

[`Thenable`](../interfaces/Thenable.md)<[`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)\>

A promise that resolves to a [document](../interfaces/codearts_plugin_.TextDocument.md).

#### Defined in

[index.d.ts:12466](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12466)

___

### registerConfiguration

▸ **registerConfiguration**(`configuration`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register configurations.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `configuration` | [`ConfigurationPropertySchema`](../interfaces/codearts_plugin_.workspace.ConfigurationPropertySchema.md) \| [`ConfigurationPropertySchema`](../interfaces/codearts_plugin_.workspace.ConfigurationPropertySchema.md)[] | The configurations to be added to the input parameter. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that deregister this configurations when being disposed.
This API complies with the JSONSchema specification and extends the configuration based on this specification.

#### Defined in

[index.d.ts:12677](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12677)

___

### registerFileSystemProvider

▸ **registerFileSystemProvider**(`scheme`, `provider`, `options?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a filesystem provider for a given scheme, e.g. `ftp`.

There can only be one provider per scheme and an error is being thrown when a scheme
has been claimed by another provider or when it is reserved.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scheme` | `string` | The uri-[scheme](../classes/codearts_plugin_.Uri.md#scheme) the provider registers for. |
| `provider` | [`FileSystemProvider`](../interfaces/codearts_plugin_.FileSystemProvider.md) | The filesystem provider. |
| `options?` | `Object` | Immutable metadata about the provider. |
| `options.isCaseSensitive?` | `boolean` | - |
| `options.isReadonly?` | `boolean` | - |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:12973](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12973)

___

### registerNotebookSerializer

▸ **registerNotebookSerializer**(`notebookType`, `serializer`, `options?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a [notebook serializer](../interfaces/codearts_plugin_.NotebookSerializer.md).

A notebook serializer must be contributed through the `notebooks` extension point. When opening a notebook file, the editor will send
the `onNotebook:<notebookType>` activation event, and extensions must register their serializer in return.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `notebookType` | `string` | A notebook. |
| `serializer` | [`NotebookSerializer`](../interfaces/codearts_plugin_.NotebookSerializer.md) | A notebook serializer. |
| `options?` | [`NotebookDocumentContentOptions`](../interfaces/codearts_plugin_.NotebookDocumentContentOptions.md) | Optional context options that define what parts of a notebook should be persisted |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this serializer when being disposed.

#### Defined in

[index.d.ts:12584](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12584)

___

### registerTaskProvider

▸ **registerTaskProvider**(`type`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a task provider.

**`Deprecated`**

Use the corresponding function on the `tasks` namespace instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `string` | The task kind type this provider is registered for. |
| `provider` | [`TaskProvider`](../interfaces/codearts_plugin_.TaskProvider.md)<[`Task`](../classes/codearts_plugin_.Task.md)\> | A task provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:12960](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12960)

___

### registerTextDocumentContentProvider

▸ **registerTextDocumentContentProvider**(`scheme`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a text document content provider.

Only one provider can be registered per scheme.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scheme` | `string` | The uri-scheme to register for. |
| `provider` | [`TextDocumentContentProvider`](../interfaces/codearts_plugin_.TextDocumentContentProvider.md) | A content provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:12477](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12477)

___

### saveAll

▸ **saveAll**(`includeUntitled?`): [`Thenable`](../interfaces/Thenable.md)<`boolean`\>

Save all dirty files.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `includeUntitled?` | `boolean` | Also save files that have been created during this session. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`boolean`\>

A thenable that resolves when the files have been saved. Will return `false`
for any file that failed to save.

#### Defined in

[index.d.ts:12403](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12403)

___

### updateConfigurationOption

▸ **updateConfigurationOption**(`target`, `key`, `value`): [`Thenable`](../interfaces/Thenable.md)<`void`\>

Update a configuration object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | ``null`` \| [`ConfigurationTarget`](../enums/codearts_plugin_.ConfigurationTarget.md) | The configuration target. |
| `key` | `string` | The key of configuration. |
| `value` | `any` | The value of configuration, type could be string, boolean, and so on. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`void`\>

#### Defined in

[index.d.ts:12944](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12944)

___

### updateWorkspaceFolders

▸ **updateWorkspaceFolders**(`start`, `deleteCount`, ...`workspaceFoldersToAdd`): `boolean`

This method replaces `deleteCount` [workspace folders](codearts_plugin_.workspace.md#workspacefolders) starting at index `start`
by an optional set of `workspaceFoldersToAdd` on the `vscode.workspace.workspaceFolders` array. This "splice"
behavior can be used to add, remove and change workspace folders in a single operation.

If the first workspace folder is added, removed or changed, the currently executing extensions (including the
one that called this method) will be terminated and restarted so that the (deprecated) `rootPath` property is
updated to point to the first workspace folder.

Use the [`onDidChangeWorkspaceFolders()`](codearts_plugin_.workspace.md#ondidchangeworkspacefolders) event to get notified when the
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

**Note:** it is not valid to call [updateWorkspaceFolders()](codearts_plugin_.workspace.md#updateworkspacefolders) multiple times
without waiting for the [`onDidChangeWorkspaceFolders()`](codearts_plugin_.workspace.md#ondidchangeworkspacefolders) to fire.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start` | `number` | the zero-based location in the list of currently opened [workspace folders](../interfaces/codearts_plugin_.WorkspaceFolder.md) from which to start deleting workspace folders. |
| `deleteCount` | `undefined` \| ``null`` \| `number` | the optional number of workspace folders to remove. |
| `...workspaceFoldersToAdd` | { `name?`: `string` ; `uri`: [`Uri`](../classes/codearts_plugin_.Uri.md)  }[] | the optional variable set of workspace folders to add in place of the deleted ones. Each workspace is identified with a mandatory URI and an optional name. |

#### Returns

`boolean`

true if the operation was successfully started and false otherwise if arguments were used that would result
in invalid workspace folder state (e.g. 2 folders with the same URI).

#### Defined in

[index.d.ts:12252](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12252)
