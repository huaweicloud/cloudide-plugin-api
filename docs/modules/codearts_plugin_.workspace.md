[@codearts/plugin](../README.md) / ["@codearts/plugin"](_codearts_plugin_.md) / workspace

# Namespace: workspace

["@codearts/plugin"](_codearts_plugin_.md).workspace

## Table of contents

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
- [registerFileSystemProvider](codearts_plugin_.workspace.md#registerfilesystemprovider)
- [registerNotebookSerializer](codearts_plugin_.workspace.md#registernotebookserializer)
- [registerTaskProvider](codearts_plugin_.workspace.md#registertaskprovider)
- [registerTextDocumentContentProvider](codearts_plugin_.workspace.md#registertextdocumentcontentprovider)
- [saveAll](codearts_plugin_.workspace.md#saveall)
- [updateWorkspaceFolders](codearts_plugin_.workspace.md#updateworkspacefolders)

## Variables

### fs

• **fs**: [`FileSystem`](../interfaces/codearts_plugin_.FileSystem.md)

#### Defined in

[index.d.ts:11592](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11592)

___

### isTrusted

• **isTrusted**: `boolean`

#### Defined in

[index.d.ts:12198](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12198)

___

### name

• **name**: `string` \| `undefined`

#### Defined in

[index.d.ts:11621](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11621)

___

### notebookDocuments

• **notebookDocuments**: readonly [`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md)[]

#### Defined in

[index.d.ts:12015](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12015)

___

### rootPath

• **rootPath**: `string` \| `undefined`

#### Defined in

[index.d.ts:11603](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11603)

___

### textDocuments

• **textDocuments**: readonly [`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)[]

#### Defined in

[index.d.ts:11906](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11906)

___

### workspaceFile

• **workspaceFile**: [`Uri`](../classes/codearts_plugin_.Uri.md) \| `undefined`

#### Defined in

[index.d.ts:11655](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11655)

___

### workspaceFolders

• **workspaceFolders**: readonly [`WorkspaceFolder`](../interfaces/codearts_plugin_.WorkspaceFolder.md)[] \| `undefined`

#### Defined in

[index.d.ts:11612](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11612)

## Functions

### applyEdit

▸ **applyEdit**(`edit`): [`Thenable`](../interfaces/Thenable.md)<`boolean`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `edit` | [`WorkspaceEdit`](../classes/codearts_plugin_.WorkspaceEdit.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`boolean`\>

#### Defined in

[index.d.ts:11901](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11901)

___

### asRelativePath

▸ **asRelativePath**(`pathOrUri`, `includeWorkspaceFolder?`): `string`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pathOrUri` | `string` \| [`Uri`](../classes/codearts_plugin_.Uri.md) |  |
| `includeWorkspaceFolder?` | `boolean` |  |

#### Returns

`string`

#### Defined in

[index.d.ts:11689](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11689)

___

### createFileSystemWatcher

▸ **createFileSystemWatcher**(`globPattern`, `ignoreCreateEvents?`, `ignoreChangeEvents?`, `ignoreDeleteEvents?`): [`FileSystemWatcher`](../interfaces/codearts_plugin_.FileSystemWatcher.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `globPattern` | [`GlobPattern`](_codearts_plugin_.md#globpattern) |  |
| `ignoreCreateEvents?` | `boolean` |  |
| `ignoreChangeEvents?` | `boolean` |  |
| `ignoreDeleteEvents?` | `boolean` |  |

#### Returns

[`FileSystemWatcher`](../interfaces/codearts_plugin_.FileSystemWatcher.md)

#### Defined in

[index.d.ts:11855](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11855)

___

### findFiles

▸ **findFiles**(`include`, `exclude?`, `maxResults?`, `token?`): [`Thenable`](../interfaces/Thenable.md)<[`Uri`](../classes/codearts_plugin_.Uri.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `include` | [`GlobPattern`](_codearts_plugin_.md#globpattern) |  |
| `exclude?` | ``null`` \| [`GlobPattern`](_codearts_plugin_.md#globpattern) |  |
| `maxResults?` | `number` |  |
| `token?` | [`CancellationToken`](../interfaces/codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`Uri`](../classes/codearts_plugin_.Uri.md)[]\>

#### Defined in

[index.d.ts:11874](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11874)

___

### getConfiguration

▸ **getConfiguration**(`section?`, `scope?`): [`WorkspaceConfiguration`](../interfaces/codearts_plugin_.WorkspaceConfiguration.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `section?` | `string` |  |
| `scope?` | ``null`` \| [`ConfigurationScope`](_codearts_plugin_.md#configurationscope) |  |

#### Returns

[`WorkspaceConfiguration`](../interfaces/codearts_plugin_.WorkspaceConfiguration.md)

#### Defined in

[index.d.ts:12164](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12164)

___

### getWorkspaceFolder

▸ **getWorkspaceFolder**(`uri`): [`WorkspaceFolder`](../interfaces/codearts_plugin_.WorkspaceFolder.md) \| `undefined`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |

#### Returns

[`WorkspaceFolder`](../interfaces/codearts_plugin_.WorkspaceFolder.md) \| `undefined`

#### Defined in

[index.d.ts:11675](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11675)

___

### onDidChangeConfiguration

▸ `Const` **onDidChangeConfiguration**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`ConfigurationChangeEvent`](../interfaces/codearts_plugin_.ConfigurationChangeEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12169](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12169)

___

### onDidChangeNotebookDocument

▸ `Const` **onDidChangeNotebookDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`NotebookDocumentChangeEvent`](../interfaces/codearts_plugin_.NotebookDocumentChangeEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12046](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12046)

___

### onDidChangeTextDocument

▸ `Const` **onDidChangeTextDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`TextDocumentChangeEvent`](../interfaces/codearts_plugin_.TextDocumentChangeEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:11990](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11990)

___

### onDidChangeWorkspaceFolders

▸ `Const` **onDidChangeWorkspaceFolders**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`WorkspaceFoldersChangeEvent`](../interfaces/codearts_plugin_.WorkspaceFoldersChangeEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:11665](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11665)

___

### onDidCloseNotebookDocument

▸ `Const` **onDidCloseNotebookDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12079](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12079)

___

### onDidCloseTextDocument

▸ `Const` **onDidCloseTextDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:11983](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11983)

___

### onDidCreateFiles

▸ `Const` **onDidCreateFiles**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`FileCreateEvent`](../interfaces/codearts_plugin_.FileCreateEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12101](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12101)

___

### onDidDeleteFiles

▸ `Const` **onDidDeleteFiles**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`FileDeleteEvent`](../interfaces/codearts_plugin_.FileDeleteEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12125](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12125)

___

### onDidGrantWorkspaceTrust

▸ `Const` **onDidGrantWorkspaceTrust**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: `void`) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12203](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12203)

___

### onDidOpenNotebookDocument

▸ `Const` **onDidOpenNotebookDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12069](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12069)

___

### onDidOpenTextDocument

▸ `Const` **onDidOpenTextDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:11971](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11971)

___

### onDidRenameFiles

▸ `Const` **onDidRenameFiles**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`FileRenameEvent`](../interfaces/codearts_plugin_.FileRenameEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12149](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12149)

___

### onDidSaveNotebookDocument

▸ `Const` **onDidSaveNotebookDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12051](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12051)

___

### onDidSaveTextDocument

▸ `Const` **onDidSaveTextDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12010](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12010)

___

### onWillCreateFiles

▸ `Const` **onWillCreateFiles**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`FileWillCreateEvent`](../interfaces/codearts_plugin_.FileWillCreateEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12091](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12091)

___

### onWillDeleteFiles

▸ `Const` **onWillDeleteFiles**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`FileWillDeleteEvent`](../interfaces/codearts_plugin_.FileWillDeleteEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12113](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12113)

___

### onWillRenameFiles

▸ `Const` **onWillRenameFiles**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`FileWillRenameEvent`](../interfaces/codearts_plugin_.FileWillRenameEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12137](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12137)

___

### onWillSaveTextDocument

▸ `Const` **onWillSaveTextDocument**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`TextDocumentWillSaveEvent`](../interfaces/codearts_plugin_.TextDocumentWillSaveEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12005](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12005)

___

### openNotebookDocument

▸ **openNotebookDocument**(`uri`): [`Thenable`](../interfaces/Thenable.md)<[`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md)\>

#### Defined in

[index.d.ts:12030](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12030)

▸ **openNotebookDocument**(`notebookType`, `content?`): [`Thenable`](../interfaces/Thenable.md)<[`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `notebookType` | `string` |  |
| `content?` | [`NotebookData`](../classes/codearts_plugin_.NotebookData.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md)\>

#### Defined in

[index.d.ts:12041](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12041)

___

### openTextDocument

▸ **openTextDocument**(`uri`): [`Thenable`](../interfaces/Thenable.md)<[`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)\>

#### Defined in

[index.d.ts:11927](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11927)

▸ **openTextDocument**(`fileName`): [`Thenable`](../interfaces/Thenable.md)<[`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fileName` | `string` |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)\>

#### Defined in

[index.d.ts:11936](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11936)

▸ **openTextDocument**(`options?`): [`Thenable`](../interfaces/Thenable.md)<[`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | `Object` |  |
| `options.content?` | `string` | - |
| `options.language?` | `string` | - |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)\>

#### Defined in

[index.d.ts:11946](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11946)

___

### registerFileSystemProvider

▸ **registerFileSystemProvider**(`scheme`, `provider`, `options?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scheme` | `string` |  |
| `provider` | [`FileSystemProvider`](../interfaces/codearts_plugin_.FileSystemProvider.md) |  |
| `options?` | `Object` |  |
| `options.isCaseSensitive?` | `boolean` | - |
| `options.isReadonly?` | `boolean` | - |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12193](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12193)

___

### registerNotebookSerializer

▸ **registerNotebookSerializer**(`notebookType`, `serializer`, `options?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `notebookType` | `string` |  |
| `serializer` | [`NotebookSerializer`](../interfaces/codearts_plugin_.NotebookSerializer.md) |  |
| `options?` | [`NotebookDocumentContentOptions`](../interfaces/codearts_plugin_.NotebookDocumentContentOptions.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12064](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12064)

___

### registerTaskProvider

▸ **registerTaskProvider**(`type`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `string` |  |
| `provider` | [`TaskProvider`](../interfaces/codearts_plugin_.TaskProvider.md)<[`Task`](../classes/codearts_plugin_.Task.md)\> |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12180](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12180)

___

### registerTextDocumentContentProvider

▸ **registerTextDocumentContentProvider**(`scheme`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scheme` | `string` |  |
| `provider` | [`TextDocumentContentProvider`](../interfaces/codearts_plugin_.TextDocumentContentProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:11957](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11957)

___

### saveAll

▸ **saveAll**(`includeUntitled?`): [`Thenable`](../interfaces/Thenable.md)<`boolean`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `includeUntitled?` | `boolean` |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`boolean`\>

#### Defined in

[index.d.ts:11883](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11883)

___

### updateWorkspaceFolders

▸ **updateWorkspaceFolders**(`start`, `deleteCount`, ...`workspaceFoldersToAdd`): `boolean`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start` | `number` |  |
| `deleteCount` | `undefined` \| ``null`` \| `number` |  |
| `...workspaceFoldersToAdd` | { `name?`: `string` ; `uri`: [`Uri`](../classes/codearts_plugin_.Uri.md)  }[] |  |

#### Returns

`boolean`

#### Defined in

[index.d.ts:11732](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11732)
