[@codearts/plugin](../README.md) / ["@codearts/plugin"](_codearts_plugin_.md) / window

# Namespace: window

["@codearts/plugin"](_codearts_plugin_.md).window

## Table of contents

### Variables

- [activeColorTheme](codearts_plugin_.window.md#activecolortheme)
- [activeNotebookEditor](codearts_plugin_.window.md#activenotebookeditor)
- [activeTerminal](codearts_plugin_.window.md#activeterminal)
- [activeTextEditor](codearts_plugin_.window.md#activetexteditor)
- [state](codearts_plugin_.window.md#state)
- [tabGroups](codearts_plugin_.window.md#tabgroups)
- [terminals](codearts_plugin_.window.md#terminals)
- [visibleNotebookEditors](codearts_plugin_.window.md#visiblenotebookeditors)
- [visibleTextEditors](codearts_plugin_.window.md#visibletexteditors)

### Functions

- [createInputBox](codearts_plugin_.window.md#createinputbox)
- [createOutputChannel](codearts_plugin_.window.md#createoutputchannel)
- [createQuickPick](codearts_plugin_.window.md#createquickpick)
- [createStatusBarItem](codearts_plugin_.window.md#createstatusbaritem)
- [createTerminal](codearts_plugin_.window.md#createterminal)
- [createTextEditorDecorationType](codearts_plugin_.window.md#createtexteditordecorationtype)
- [createTreeView](codearts_plugin_.window.md#createtreeview)
- [createWebviewPanel](codearts_plugin_.window.md#createwebviewpanel)
- [onDidChangeActiveColorTheme](codearts_plugin_.window.md#ondidchangeactivecolortheme)
- [onDidChangeActiveNotebookEditor](codearts_plugin_.window.md#ondidchangeactivenotebookeditor)
- [onDidChangeActiveTerminal](codearts_plugin_.window.md#ondidchangeactiveterminal)
- [onDidChangeActiveTextEditor](codearts_plugin_.window.md#ondidchangeactivetexteditor)
- [onDidChangeNotebookEditorSelection](codearts_plugin_.window.md#ondidchangenotebookeditorselection)
- [onDidChangeNotebookEditorVisibleRanges](codearts_plugin_.window.md#ondidchangenotebookeditorvisibleranges)
- [onDidChangeTerminalState](codearts_plugin_.window.md#ondidchangeterminalstate)
- [onDidChangeTextEditorOptions](codearts_plugin_.window.md#ondidchangetexteditoroptions)
- [onDidChangeTextEditorSelection](codearts_plugin_.window.md#ondidchangetexteditorselection)
- [onDidChangeTextEditorViewColumn](codearts_plugin_.window.md#ondidchangetexteditorviewcolumn)
- [onDidChangeTextEditorVisibleRanges](codearts_plugin_.window.md#ondidchangetexteditorvisibleranges)
- [onDidChangeVisibleNotebookEditors](codearts_plugin_.window.md#ondidchangevisiblenotebookeditors)
- [onDidChangeVisibleTextEditors](codearts_plugin_.window.md#ondidchangevisibletexteditors)
- [onDidChangeWindowState](codearts_plugin_.window.md#ondidchangewindowstate)
- [onDidCloseTerminal](codearts_plugin_.window.md#ondidcloseterminal)
- [onDidOpenTerminal](codearts_plugin_.window.md#ondidopenterminal)
- [registerCustomEditorProvider](codearts_plugin_.window.md#registercustomeditorprovider)
- [registerFileDecorationProvider](codearts_plugin_.window.md#registerfiledecorationprovider)
- [registerTerminalLinkProvider](codearts_plugin_.window.md#registerterminallinkprovider)
- [registerTerminalProfileProvider](codearts_plugin_.window.md#registerterminalprofileprovider)
- [registerTreeDataProvider](codearts_plugin_.window.md#registertreedataprovider)
- [registerUriHandler](codearts_plugin_.window.md#registerurihandler)
- [registerWebviewPanelSerializer](codearts_plugin_.window.md#registerwebviewpanelserializer)
- [registerWebviewViewProvider](codearts_plugin_.window.md#registerwebviewviewprovider)
- [setStatusBarMessage](codearts_plugin_.window.md#setstatusbarmessage)
- [showErrorMessage](codearts_plugin_.window.md#showerrormessage)
- [showInformationMessage](codearts_plugin_.window.md#showinformationmessage)
- [showInputBox](codearts_plugin_.window.md#showinputbox)
- [showNotebookDocument](codearts_plugin_.window.md#shownotebookdocument)
- [showOpenDialog](codearts_plugin_.window.md#showopendialog)
- [showQuickPick](codearts_plugin_.window.md#showquickpick)
- [showSaveDialog](codearts_plugin_.window.md#showsavedialog)
- [showTextDocument](codearts_plugin_.window.md#showtextdocument)
- [showWarningMessage](codearts_plugin_.window.md#showwarningmessage)
- [showWorkspaceFolderPick](codearts_plugin_.window.md#showworkspacefolderpick)
- [withProgress](codearts_plugin_.window.md#withprogress)
- [withScmProgress](codearts_plugin_.window.md#withscmprogress)

## Variables

### activeColorTheme

• **activeColorTheme**: [`ColorTheme`](../interfaces/codearts_plugin_.ColorTheme.md)

#### Defined in

[index.d.ts:9996](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9996)

___

### activeNotebookEditor

• **activeNotebookEditor**: [`NotebookEditor`](../interfaces/codearts_plugin_.NotebookEditor.md) \| `undefined`

#### Defined in

[index.d.ts:9348](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9348)

___

### activeTerminal

• **activeTerminal**: [`Terminal`](../interfaces/codearts_plugin_.Terminal.md) \| `undefined`

#### Defined in

[index.d.ts:9378](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9378)

___

### activeTextEditor

• **activeTextEditor**: [`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md) \| `undefined`

#### Defined in

[index.d.ts:9292](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9292)

___

### state

• **state**: [`WindowState`](../interfaces/codearts_plugin_.WindowState.md)

#### Defined in

[index.d.ts:9406](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9406)

___

### tabGroups

• **tabGroups**: [`TabGroups`](../interfaces/codearts_plugin_.TabGroups.md)

#### Defined in

[index.d.ts:9285](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9285)

___

### terminals

• **terminals**: readonly [`Terminal`](../interfaces/codearts_plugin_.Terminal.md)[]

#### Defined in

[index.d.ts:9372](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9372)

___

### visibleNotebookEditors

• **visibleNotebookEditors**: readonly [`NotebookEditor`](../interfaces/codearts_plugin_.NotebookEditor.md)[]

#### Defined in

[index.d.ts:9335](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9335)

___

### visibleTextEditors

• **visibleTextEditors**: readonly [`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)[]

#### Defined in

[index.d.ts:9297](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9297)

## Functions

### createInputBox

▸ **createInputBox**(): [`InputBox`](../interfaces/codearts_plugin_.InputBox.md)

#### Returns

[`InputBox`](../interfaces/codearts_plugin_.InputBox.md)

#### Defined in

[index.d.ts:9703](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9703)

___

### createOutputChannel

▸ **createOutputChannel**(`name`, `languageId?`): [`OutputChannel`](../interfaces/codearts_plugin_.OutputChannel.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` |  |
| `languageId?` | `string` |  |

#### Returns

[`OutputChannel`](../interfaces/codearts_plugin_.OutputChannel.md)

#### Defined in

[index.d.ts:9715](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9715)

___

### createQuickPick

▸ **createQuickPick**<`T`\>(): [`QuickPick`](../interfaces/codearts_plugin_.QuickPick.md)<`T`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`QuickPickItem`](../interfaces/codearts_plugin_.QuickPickItem.md) |

#### Returns

[`QuickPick`](../interfaces/codearts_plugin_.QuickPick.md)<`T`\>

#### Defined in

[index.d.ts:9692](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9692)

___

### createStatusBarItem

▸ **createStatusBarItem**(`alignment?`, `priority?`): [`StatusBarItem`](../interfaces/codearts_plugin_.StatusBarItem.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `alignment?` | [`StatusBarAlignment`](../enums/codearts_plugin_.StatusBarAlignment.md) |  |
| `priority?` | `number` |  |

#### Returns

[`StatusBarItem`](../interfaces/codearts_plugin_.StatusBarItem.md)

#### Defined in

[index.d.ts:9801](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9801)

▸ **createStatusBarItem**(`id`, `alignment?`, `priority?`): [`StatusBarItem`](../interfaces/codearts_plugin_.StatusBarItem.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` |  |
| `alignment?` | [`StatusBarAlignment`](../enums/codearts_plugin_.StatusBarAlignment.md) |  |
| `priority?` | `number` |  |

#### Returns

[`StatusBarItem`](../interfaces/codearts_plugin_.StatusBarItem.md)

#### Defined in

[index.d.ts:9811](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9811)

___

### createTerminal

▸ **createTerminal**(`name?`, `shellPath?`, `shellArgs?`): [`Terminal`](../interfaces/codearts_plugin_.Terminal.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name?` | `string` |  |
| `shellPath?` | `string` |  |
| `shellArgs?` | `string` \| readonly `string`[] |  |

#### Returns

[`Terminal`](../interfaces/codearts_plugin_.Terminal.md)

#### Defined in

[index.d.ts:9825](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9825)

▸ **createTerminal**(`options`): [`Terminal`](../interfaces/codearts_plugin_.Terminal.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`TerminalOptions`](../interfaces/codearts_plugin_.TerminalOptions.md) |  |

#### Returns

[`Terminal`](../interfaces/codearts_plugin_.Terminal.md)

#### Defined in

[index.d.ts:9834](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9834)

▸ **createTerminal**(`options`): [`Terminal`](../interfaces/codearts_plugin_.Terminal.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`ExtensionTerminalOptions`](../interfaces/codearts_plugin_.ExtensionTerminalOptions.md) |  |

#### Returns

[`Terminal`](../interfaces/codearts_plugin_.Terminal.md)

#### Defined in

[index.d.ts:9843](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9843)

___

### createTextEditorDecorationType

▸ **createTextEditorDecorationType**(`options`): [`TextEditorDecorationType`](../interfaces/codearts_plugin_.TextEditorDecorationType.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`DecorationRenderOptions`](../interfaces/codearts_plugin_.DecorationRenderOptions.md) |  |

#### Returns

[`TextEditorDecorationType`](../interfaces/codearts_plugin_.TextEditorDecorationType.md)

#### Defined in

[index.d.ts:9464](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9464)

___

### createTreeView

▸ **createTreeView**<`T`\>(`viewId`, `options`): [`TreeView`](../interfaces/codearts_plugin_.TreeView.md)<`T`\>

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewId` | `string` |  |
| `options` | [`TreeViewOptions`](../interfaces/codearts_plugin_.TreeViewOptions.md)<`T`\> |  |

#### Returns

[`TreeView`](../interfaces/codearts_plugin_.TreeView.md)<`T`\>

#### Defined in

[index.d.ts:9862](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9862)

___

### createWebviewPanel

▸ **createWebviewPanel**(`viewType`, `title`, `showOptions`, `options?`): [`WebviewPanel`](../interfaces/codearts_plugin_.WebviewPanel.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewType` | `string` |  |
| `title` | `string` |  |
| `showOptions` | [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md) \| { `preserveFocus?`: `boolean` ; `viewColumn`: [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md)  } |  |
| `options?` | [`WebviewPanelOptions`](../interfaces/codearts_plugin_.WebviewPanelOptions.md) & [`WebviewOptions`](../interfaces/codearts_plugin_.WebviewOptions.md) |  |

#### Returns

[`WebviewPanel`](../interfaces/codearts_plugin_.WebviewPanel.md)

#### Defined in

[index.d.ts:9727](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9727)

___

### onDidChangeActiveColorTheme

▸ `Const` **onDidChangeActiveColorTheme**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`ColorTheme`](../interfaces/codearts_plugin_.ColorTheme.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:10001](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L10001)

___

### onDidChangeActiveNotebookEditor

▸ `Const` **onDidChangeActiveNotebookEditor**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: `undefined` \| [`NotebookEditor`](../interfaces/codearts_plugin_.NotebookEditor.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9355](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9355)

___

### onDidChangeActiveTerminal

▸ `Const` **onDidChangeActiveTerminal**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: `undefined` \| [`Terminal`](../interfaces/codearts_plugin_.Terminal.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9385](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9385)

___

### onDidChangeActiveTextEditor

▸ `Const` **onDidChangeActiveTextEditor**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: `undefined` \| [`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9304](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9304)

___

### onDidChangeNotebookEditorSelection

▸ `Const` **onDidChangeNotebookEditorSelection**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`NotebookEditorSelectionChangeEvent`](../interfaces/codearts_plugin_.NotebookEditorSelectionChangeEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9361](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9361)

___

### onDidChangeNotebookEditorVisibleRanges

▸ `Const` **onDidChangeNotebookEditorVisibleRanges**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`NotebookEditorVisibleRangesChangeEvent`](../interfaces/codearts_plugin_.NotebookEditorVisibleRangesChangeEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9367](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9367)

___

### onDidChangeTerminalState

▸ `Const` **onDidChangeTerminalState**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`Terminal`](../interfaces/codearts_plugin_.Terminal.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9401](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9401)

___

### onDidChangeTextEditorOptions

▸ `Const` **onDidChangeTextEditorOptions**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`TextEditorOptionsChangeEvent`](../interfaces/codearts_plugin_.TextEditorOptionsChangeEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9325](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9325)

___

### onDidChangeTextEditorSelection

▸ `Const` **onDidChangeTextEditorSelection**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`TextEditorSelectionChangeEvent`](../interfaces/codearts_plugin_.TextEditorSelectionChangeEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9315](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9315)

___

### onDidChangeTextEditorViewColumn

▸ `Const` **onDidChangeTextEditorViewColumn**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`TextEditorViewColumnChangeEvent`](../interfaces/codearts_plugin_.TextEditorViewColumnChangeEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9330](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9330)

___

### onDidChangeTextEditorVisibleRanges

▸ `Const` **onDidChangeTextEditorVisibleRanges**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`TextEditorVisibleRangesChangeEvent`](../interfaces/codearts_plugin_.TextEditorVisibleRangesChangeEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9320](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9320)

___

### onDidChangeVisibleNotebookEditors

▸ `Const` **onDidChangeVisibleNotebookEditors**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: readonly [`NotebookEditor`](../interfaces/codearts_plugin_.NotebookEditor.md)[]) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9341](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9341)

___

### onDidChangeVisibleTextEditors

▸ `Const` **onDidChangeVisibleTextEditors**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: readonly [`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)[]) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9310](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9310)

___

### onDidChangeWindowState

▸ `Const` **onDidChangeWindowState**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`WindowState`](../interfaces/codearts_plugin_.WindowState.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9412](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9412)

___

### onDidCloseTerminal

▸ `Const` **onDidCloseTerminal**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`Terminal`](../interfaces/codearts_plugin_.Terminal.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9396](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9396)

___

### onDidOpenTerminal

▸ `Const` **onDidOpenTerminal**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`Terminal`](../interfaces/codearts_plugin_.Terminal.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9391](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9391)

___

### registerCustomEditorProvider

▸ **registerCustomEditorProvider**(`viewType`, `provider`, `options?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewType` | `string` |  |
| `provider` | [`CustomTextEditorProvider`](../interfaces/codearts_plugin_.CustomTextEditorProvider.md) \| [`CustomReadonlyEditorProvider`](../interfaces/codearts_plugin_.CustomReadonlyEditorProvider.md)<[`CustomDocument`](../interfaces/codearts_plugin_.CustomDocument.md)\> \| [`CustomEditorProvider`](../interfaces/codearts_plugin_.CustomEditorProvider.md)<[`CustomDocument`](../interfaces/codearts_plugin_.CustomDocument.md)\> |  |
| `options?` | `Object` |  |
| `options.supportsMultipleEditorsPerDocument?` | `boolean` |  |
| `options.webviewOptions?` | [`WebviewPanelOptions`](../interfaces/codearts_plugin_.WebviewPanelOptions.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9948](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9948)

___

### registerFileDecorationProvider

▸ **registerFileDecorationProvider**(`provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `provider` | [`FileDecorationProvider`](../interfaces/codearts_plugin_.FileDecorationProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9990](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9990)

___

### registerTerminalLinkProvider

▸ **registerTerminalLinkProvider**(`provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `provider` | [`TerminalLinkProvider`](../interfaces/codearts_plugin_.TerminalLinkProvider.md)<[`TerminalLink`](../classes/codearts_plugin_.TerminalLink.md)\> |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9976](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9976)

___

### registerTerminalProfileProvider

▸ **registerTerminalProfileProvider**(`id`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` |  |
| `provider` | [`TerminalProfileProvider`](../interfaces/codearts_plugin_.TerminalProfileProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9983](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9983)

___

### registerTreeDataProvider

▸ **registerTreeDataProvider**<`T`\>(`viewId`, `treeDataProvider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewId` | `string` |  |
| `treeDataProvider` | [`TreeDataProvider`](../interfaces/codearts_plugin_.TreeDataProvider.md)<`T`\> |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9854](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9854)

___

### registerUriHandler

▸ **registerUriHandler**(`handler`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `handler` | [`UriHandler`](../interfaces/codearts_plugin_.UriHandler.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9885](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9885)

___

### registerWebviewPanelSerializer

▸ **registerWebviewPanelSerializer**(`viewType`, `serializer`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewType` | `string` |  |
| `serializer` | [`WebviewPanelSerializer`](../interfaces/codearts_plugin_.WebviewPanelSerializer.md)<`unknown`\> |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9898](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9898)

___

### registerWebviewViewProvider

▸ **registerWebviewViewProvider**(`viewId`, `provider`, `options?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewId` | `string` |  |
| `provider` | [`WebviewViewProvider`](../interfaces/codearts_plugin_.WebviewViewProvider.md) |  |
| `options?` | `Object` | - |
| `options.webviewOptions?` | `Object` |  |
| `options.webviewOptions.retainContextWhenHidden?` | `boolean` |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9909](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9909)

___

### setStatusBarMessage

▸ **setStatusBarMessage**(`text`, `hideAfterTimeout`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` |  |
| `hideAfterTimeout` | `number` |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9737](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9737)

▸ **setStatusBarMessage**(`text`, `hideWhenDone`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` |  |
| `hideWhenDone` | [`Thenable`](../interfaces/Thenable.md)<`any`\> |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9747](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9747)

▸ **setStatusBarMessage**(`text`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9759](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9759)

___

### showErrorMessage

▸ **showErrorMessage**<`T`\>(`message`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `string` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` |  |
| `...items` | `T`[] |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Defined in

[index.d.ts:9565](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9565)

▸ **showErrorMessage**<`T`\>(`message`, `options`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `string` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` |  |
| `options` | [`MessageOptions`](../interfaces/codearts_plugin_.MessageOptions.md) |  |
| `...items` | `T`[] |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Defined in

[index.d.ts:9577](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9577)

▸ **showErrorMessage**<`T`\>(`message`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`MessageItem`](../interfaces/codearts_plugin_.MessageItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` |  |
| `...items` | `T`[] |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Defined in

[index.d.ts:9588](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9588)

▸ **showErrorMessage**<`T`\>(`message`, `options`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`MessageItem`](../interfaces/codearts_plugin_.MessageItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` |  |
| `options` | [`MessageOptions`](../interfaces/codearts_plugin_.MessageOptions.md) |  |
| `...items` | `T`[] |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Defined in

[index.d.ts:9600](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9600)

___

### showInformationMessage

▸ **showInformationMessage**<`T`\>(`message`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `string` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` |  |
| `...items` | `T`[] |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Defined in

[index.d.ts:9474](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9474)

▸ **showInformationMessage**<`T`\>(`message`, `options`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `string` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` |  |
| `options` | [`MessageOptions`](../interfaces/codearts_plugin_.MessageOptions.md) |  |
| `...items` | `T`[] |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Defined in

[index.d.ts:9485](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9485)

▸ **showInformationMessage**<`T`\>(`message`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`MessageItem`](../interfaces/codearts_plugin_.MessageItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` |  |
| `...items` | `T`[] |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Defined in

[index.d.ts:9496](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9496)

▸ **showInformationMessage**<`T`\>(`message`, `options`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`MessageItem`](../interfaces/codearts_plugin_.MessageItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` |  |
| `options` | [`MessageOptions`](../interfaces/codearts_plugin_.MessageOptions.md) |  |
| `...items` | `T`[] |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Defined in

[index.d.ts:9508](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9508)

___

### showInputBox

▸ **showInputBox**(`options?`, `token?`): [`Thenable`](../interfaces/Thenable.md)<`string` \| `undefined`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | [`InputBoxOptions`](../interfaces/codearts_plugin_.InputBoxOptions.md) |  |
| `token?` | [`CancellationToken`](../interfaces/codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`string` \| `undefined`\>

#### Defined in

[index.d.ts:9680](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9680)

___

### showNotebookDocument

▸ **showNotebookDocument**(`document`, `options?`): [`Thenable`](../interfaces/Thenable.md)<[`NotebookEditor`](../interfaces/codearts_plugin_.NotebookEditor.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md) |  |
| `options?` | [`NotebookDocumentShowOptions`](../interfaces/codearts_plugin_.NotebookDocumentShowOptions.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`NotebookEditor`](../interfaces/codearts_plugin_.NotebookEditor.md)\>

#### Defined in

[index.d.ts:9456](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9456)

___

### showOpenDialog

▸ **showOpenDialog**(`options?`): [`Thenable`](../interfaces/Thenable.md)<[`Uri`](../classes/codearts_plugin_.Uri.md)[] \| `undefined`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | [`OpenDialogOptions`](../interfaces/codearts_plugin_.OpenDialogOptions.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`Uri`](../classes/codearts_plugin_.Uri.md)[] \| `undefined`\>

#### Defined in

[index.d.ts:9658](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9658)

___

### showQuickPick

▸ **showQuickPick**(`items`, `options`, `token?`): [`Thenable`](../interfaces/Thenable.md)<`string`[] \| `undefined`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `items` | readonly `string`[] \| [`Thenable`](../interfaces/Thenable.md)<readonly `string`[]\> |  |
| `options` | [`QuickPickOptions`](../interfaces/codearts_plugin_.QuickPickOptions.md) & { `canPickMany`: ``true``  } |  |
| `token?` | [`CancellationToken`](../interfaces/codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`string`[] \| `undefined`\>

#### Defined in

[index.d.ts:9610](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9610)

▸ **showQuickPick**(`items`, `options?`, `token?`): [`Thenable`](../interfaces/Thenable.md)<`string` \| `undefined`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `items` | readonly `string`[] \| [`Thenable`](../interfaces/Thenable.md)<readonly `string`[]\> |  |
| `options?` | [`QuickPickOptions`](../interfaces/codearts_plugin_.QuickPickOptions.md) |  |
| `token?` | [`CancellationToken`](../interfaces/codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`string` \| `undefined`\>

#### Defined in

[index.d.ts:9620](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9620)

▸ **showQuickPick**<`T`\>(`items`, `options`, `token?`): [`Thenable`](../interfaces/Thenable.md)<`T`[] \| `undefined`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`QuickPickItem`](../interfaces/codearts_plugin_.QuickPickItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `items` | readonly `T`[] \| [`Thenable`](../interfaces/Thenable.md)<readonly `T`[]\> |  |
| `options` | [`QuickPickOptions`](../interfaces/codearts_plugin_.QuickPickOptions.md) & { `canPickMany`: ``true``  } |  |
| `token?` | [`CancellationToken`](../interfaces/codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T`[] \| `undefined`\>

#### Defined in

[index.d.ts:9630](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9630)

▸ **showQuickPick**<`T`\>(`items`, `options?`, `token?`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`QuickPickItem`](../interfaces/codearts_plugin_.QuickPickItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `items` | readonly `T`[] \| [`Thenable`](../interfaces/Thenable.md)<readonly `T`[]\> |  |
| `options?` | [`QuickPickOptions`](../interfaces/codearts_plugin_.QuickPickOptions.md) |  |
| `token?` | [`CancellationToken`](../interfaces/codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Defined in

[index.d.ts:9640](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9640)

___

### showSaveDialog

▸ **showSaveDialog**(`options?`): [`Thenable`](../interfaces/Thenable.md)<[`Uri`](../classes/codearts_plugin_.Uri.md) \| `undefined`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | [`SaveDialogOptions`](../interfaces/codearts_plugin_.SaveDialogOptions.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`Uri`](../classes/codearts_plugin_.Uri.md) \| `undefined`\>

#### Defined in

[index.d.ts:9667](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9667)

___

### showTextDocument

▸ **showTextDocument**(`document`, `column?`, `preserveFocus?`): [`Thenable`](../interfaces/Thenable.md)<[`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md) |  |
| `column?` | [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md) |  |
| `preserveFocus?` | `boolean` |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)\>

#### Defined in

[index.d.ts:9425](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9425)

▸ **showTextDocument**(`document`, `options?`): [`Thenable`](../interfaces/Thenable.md)<[`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md) |  |
| `options?` | [`TextDocumentShowOptions`](../interfaces/codearts_plugin_.TextDocumentShowOptions.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)\>

#### Defined in

[index.d.ts:9435](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9435)

▸ **showTextDocument**(`uri`, `options?`): [`Thenable`](../interfaces/Thenable.md)<[`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |
| `options?` | [`TextDocumentShowOptions`](../interfaces/codearts_plugin_.TextDocumentShowOptions.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)\>

#### Defined in

[index.d.ts:9446](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9446)

___

### showWarningMessage

▸ **showWarningMessage**<`T`\>(`message`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `string` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` |  |
| `...items` | `T`[] |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Defined in

[index.d.ts:9519](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9519)

▸ **showWarningMessage**<`T`\>(`message`, `options`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `string` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` |  |
| `options` | [`MessageOptions`](../interfaces/codearts_plugin_.MessageOptions.md) |  |
| `...items` | `T`[] |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Defined in

[index.d.ts:9531](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9531)

▸ **showWarningMessage**<`T`\>(`message`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`MessageItem`](../interfaces/codearts_plugin_.MessageItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` |  |
| `...items` | `T`[] |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Defined in

[index.d.ts:9542](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9542)

▸ **showWarningMessage**<`T`\>(`message`, `options`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`MessageItem`](../interfaces/codearts_plugin_.MessageItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` |  |
| `options` | [`MessageOptions`](../interfaces/codearts_plugin_.MessageOptions.md) |  |
| `...items` | `T`[] |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

#### Defined in

[index.d.ts:9554](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9554)

___

### showWorkspaceFolderPick

▸ **showWorkspaceFolderPick**(`options?`): [`Thenable`](../interfaces/Thenable.md)<[`WorkspaceFolder`](../interfaces/codearts_plugin_.WorkspaceFolder.md) \| `undefined`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | [`WorkspaceFolderPickOptions`](../interfaces/codearts_plugin_.WorkspaceFolderPickOptions.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`WorkspaceFolder`](../interfaces/codearts_plugin_.WorkspaceFolder.md) \| `undefined`\>

#### Defined in

[index.d.ts:9649](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9649)

___

### withProgress

▸ **withProgress**<`R`\>(`options`, `task`): [`Thenable`](../interfaces/Thenable.md)<`R`\>

#### Type parameters

| Name |
| :------ |
| `R` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`ProgressOptions`](../interfaces/codearts_plugin_.ProgressOptions.md) | - |
| `task` | (`progress`: [`Progress`](../interfaces/codearts_plugin_.Progress.md)<{ `increment?`: `number` ; `message?`: `string`  }\>, `token`: [`CancellationToken`](../interfaces/codearts_plugin_.CancellationToken.md)) => [`Thenable`](../interfaces/Thenable.md)<`R`\> |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`R`\>

#### Defined in

[index.d.ts:9792](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9792)

___

### withScmProgress

▸ **withScmProgress**<`R`\>(`task`): [`Thenable`](../interfaces/Thenable.md)<`R`\>

#### Type parameters

| Name |
| :------ |
| `R` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `task` | (`progress`: [`Progress`](../interfaces/codearts_plugin_.Progress.md)<`number`\>) => [`Thenable`](../interfaces/Thenable.md)<`R`\> |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`R`\>

#### Defined in

[index.d.ts:9771](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L9771)
