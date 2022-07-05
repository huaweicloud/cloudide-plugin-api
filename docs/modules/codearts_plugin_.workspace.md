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

[index.d.ts:11562](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11562)

___

### isTrusted

• **isTrusted**: `boolean`

#### Defined in

[index.d.ts:12168](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12168)

___

### name

• **name**: `string` \| `undefined`

#### Defined in

[index.d.ts:11591](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11591)

___

### notebookDocuments

• **notebookDocuments**: readonly [`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md)[]

#### Defined in

[index.d.ts:11985](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11985)

___

### rootPath

• **rootPath**: `string` \| `undefined`

#### Defined in

[index.d.ts:11573](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11573)

___

### textDocuments

• **textDocuments**: readonly [`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)[]

#### Defined in

[index.d.ts:11876](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11876)

___

### workspaceFile

• **workspaceFile**: [`Uri`](../classes/codearts_plugin_.Uri.md) \| `undefined`

#### Defined in

[index.d.ts:11625](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11625)

___

### workspaceFolders

• **workspaceFolders**: readonly [`WorkspaceFolder`](../interfaces/codearts_plugin_.WorkspaceFolder.md)[] \| `undefined`

#### Defined in

[index.d.ts:11582](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11582)

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

[index.d.ts:11871](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11871)

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

[index.d.ts:11659](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11659)

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

[index.d.ts:11825](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11825)

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

[index.d.ts:11844](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11844)

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

[index.d.ts:12134](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12134)

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

[index.d.ts:11645](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11645)

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

[index.d.ts:12139](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12139)

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

[index.d.ts:12016](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12016)

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

[index.d.ts:11960](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11960)

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

[index.d.ts:11635](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11635)

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

[index.d.ts:12049](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12049)

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

[index.d.ts:11953](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11953)

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

[index.d.ts:12071](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12071)

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

[index.d.ts:12095](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12095)

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

[index.d.ts:12173](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12173)

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

[index.d.ts:12039](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12039)

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

[index.d.ts:11941](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11941)

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

[index.d.ts:12119](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12119)

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

[index.d.ts:12021](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12021)

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

[index.d.ts:11980](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11980)

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

[index.d.ts:12061](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12061)

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

[index.d.ts:12083](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12083)

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

[index.d.ts:12107](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12107)

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

[index.d.ts:11975](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11975)

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

[index.d.ts:12000](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12000)

▸ **openNotebookDocument**(`notebookType`, `content?`): [`Thenable`](../interfaces/Thenable.md)<[`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `notebookType` | `string` |  |
| `content?` | [`NotebookData`](../classes/codearts_plugin_.NotebookData.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md)\>

#### Defined in

[index.d.ts:12011](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12011)

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

[index.d.ts:11897](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11897)

▸ **openTextDocument**(`fileName`): [`Thenable`](../interfaces/Thenable.md)<[`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fileName` | `string` |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)\>

#### Defined in

[index.d.ts:11906](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11906)

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

[index.d.ts:11916](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11916)

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

[index.d.ts:12163](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12163)

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

[index.d.ts:12034](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12034)

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

[index.d.ts:12150](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12150)

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

[index.d.ts:11927](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11927)

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

[index.d.ts:11853](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11853)

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

[index.d.ts:11702](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L11702)
