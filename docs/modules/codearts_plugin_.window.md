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
- [createLightWebviewPanel](codearts_plugin_.window.md#createlightwebviewpanel)
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

[index.d.ts:10026](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10026)

___

### activeNotebookEditor

• **activeNotebookEditor**: [`NotebookEditor`](../interfaces/codearts_plugin_.NotebookEditor.md) \| `undefined`

#### Defined in

[index.d.ts:9366](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9366)

___

### activeTerminal

• **activeTerminal**: [`Terminal`](../interfaces/codearts_plugin_.Terminal.md) \| `undefined`

#### Defined in

[index.d.ts:9396](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9396)

___

### activeTextEditor

• **activeTextEditor**: [`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md) \| `undefined`

#### Defined in

[index.d.ts:9310](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9310)

___

### state

• **state**: [`WindowState`](../interfaces/codearts_plugin_.WindowState.md)

#### Defined in

[index.d.ts:9424](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9424)

___

### tabGroups

• **tabGroups**: [`TabGroups`](../interfaces/codearts_plugin_.TabGroups.md)

#### Defined in

[index.d.ts:9303](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9303)

___

### terminals

• **terminals**: readonly [`Terminal`](../interfaces/codearts_plugin_.Terminal.md)[]

#### Defined in

[index.d.ts:9390](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9390)

___

### visibleNotebookEditors

• **visibleNotebookEditors**: readonly [`NotebookEditor`](../interfaces/codearts_plugin_.NotebookEditor.md)[]

#### Defined in

[index.d.ts:9353](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9353)

___

### visibleTextEditors

• **visibleTextEditors**: readonly [`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)[]

#### Defined in

[index.d.ts:9315](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9315)

## Functions

### createInputBox

▸ **createInputBox**(): [`InputBox`](../interfaces/codearts_plugin_.InputBox.md)

#### Returns

[`InputBox`](../interfaces/codearts_plugin_.InputBox.md)

#### Defined in

[index.d.ts:9721](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9721)

___

### createLightWebviewPanel

▸ **createLightWebviewPanel**(`viewType`, `title`, `showOptions`, `options?`): [`WebviewPanel`](../interfaces/codearts_plugin_.WebviewPanel.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewType` | `string` |  |
| `title` | `string` |  |
| `showOptions` | [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md) \| { `area`: `string` ; `preserveFocus?`: `boolean` ; `viewColumn?`: [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md)  } |  |
| `options?` | [`WebviewPanelOptions`](../interfaces/codearts_plugin_.WebviewPanelOptions.md) & [`WebviewOptions`](../interfaces/codearts_plugin_.WebviewOptions.md) |  |

#### Returns

[`WebviewPanel`](../interfaces/codearts_plugin_.WebviewPanel.md)

#### Defined in

[index.d.ts:9757](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9757)

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

[index.d.ts:9733](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9733)

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

[index.d.ts:9710](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9710)

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

[index.d.ts:9831](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9831)

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

[index.d.ts:9841](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9841)

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

[index.d.ts:9855](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9855)

▸ **createTerminal**(`options`): [`Terminal`](../interfaces/codearts_plugin_.Terminal.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`TerminalOptions`](../interfaces/codearts_plugin_.TerminalOptions.md) |  |

#### Returns

[`Terminal`](../interfaces/codearts_plugin_.Terminal.md)

#### Defined in

[index.d.ts:9864](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9864)

▸ **createTerminal**(`options`): [`Terminal`](../interfaces/codearts_plugin_.Terminal.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`ExtensionTerminalOptions`](../interfaces/codearts_plugin_.ExtensionTerminalOptions.md) |  |

#### Returns

[`Terminal`](../interfaces/codearts_plugin_.Terminal.md)

#### Defined in

[index.d.ts:9873](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9873)

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

[index.d.ts:9482](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9482)

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

[index.d.ts:9892](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9892)

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

[index.d.ts:9745](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9745)

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

[index.d.ts:10031](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10031)

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

[index.d.ts:9373](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9373)

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

[index.d.ts:9403](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9403)

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

[index.d.ts:9322](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9322)

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

[index.d.ts:9379](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9379)

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

[index.d.ts:9385](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9385)

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

[index.d.ts:9419](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9419)

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

[index.d.ts:9343](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9343)

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

[index.d.ts:9333](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9333)

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

[index.d.ts:9348](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9348)

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

[index.d.ts:9338](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9338)

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

[index.d.ts:9359](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9359)

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

[index.d.ts:9328](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9328)

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

[index.d.ts:9430](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9430)

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

[index.d.ts:9414](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9414)

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

[index.d.ts:9409](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9409)

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

[index.d.ts:9978](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9978)

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

[index.d.ts:10020](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10020)

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

[index.d.ts:10006](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10006)

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

[index.d.ts:10013](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10013)

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

[index.d.ts:9884](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9884)

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

[index.d.ts:9915](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9915)

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

[index.d.ts:9928](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9928)

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

[index.d.ts:9939](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9939)

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

[index.d.ts:9767](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9767)

▸ **setStatusBarMessage**(`text`, `hideWhenDone`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` |  |
| `hideWhenDone` | [`Thenable`](../interfaces/Thenable.md)<`any`\> |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9777](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9777)

▸ **setStatusBarMessage**(`text`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9789](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9789)

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

[index.d.ts:9583](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9583)

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

[index.d.ts:9595](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9595)

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

[index.d.ts:9606](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9606)

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

[index.d.ts:9618](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9618)

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

[index.d.ts:9492](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9492)

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

[index.d.ts:9503](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9503)

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

[index.d.ts:9514](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9514)

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

[index.d.ts:9526](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9526)

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

[index.d.ts:9698](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9698)

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

[index.d.ts:9474](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9474)

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

[index.d.ts:9676](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9676)

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

[index.d.ts:9628](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9628)

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

[index.d.ts:9638](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9638)

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

[index.d.ts:9648](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9648)

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

[index.d.ts:9658](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9658)

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

[index.d.ts:9685](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9685)

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

[index.d.ts:9443](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9443)

▸ **showTextDocument**(`document`, `options?`): [`Thenable`](../interfaces/Thenable.md)<[`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md) |  |
| `options?` | [`TextDocumentShowOptions`](../interfaces/codearts_plugin_.TextDocumentShowOptions.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)\>

#### Defined in

[index.d.ts:9453](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9453)

▸ **showTextDocument**(`uri`, `options?`): [`Thenable`](../interfaces/Thenable.md)<[`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |
| `options?` | [`TextDocumentShowOptions`](../interfaces/codearts_plugin_.TextDocumentShowOptions.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)\>

#### Defined in

[index.d.ts:9464](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9464)

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

[index.d.ts:9537](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9537)

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

[index.d.ts:9549](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9549)

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

[index.d.ts:9560](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9560)

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

[index.d.ts:9572](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9572)

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

[index.d.ts:9667](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9667)

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

[index.d.ts:9822](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9822)

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

[index.d.ts:9801](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9801)
