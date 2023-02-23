[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](_cloudide_plugin_.md) / window

# Namespace: window

["@cloudide/plugin"](_cloudide_plugin_.md).window

Common namespace for dealing with window and editor, showing messages and user input.

## Table of contents

### Interfaces

- [CustomizableDialog](../interfaces/cloudide_plugin_.window.CustomizableDialog.md)
- [CustomizableDialogEvent](../interfaces/cloudide_plugin_.window.CustomizableDialogEvent.md)
- [CustomizableDialogOptions](../interfaces/cloudide_plugin_.window.CustomizableDialogOptions.md)
- [DialogButton](../interfaces/cloudide_plugin_.window.DialogButton.md)
- [DialogControlElement](../interfaces/cloudide_plugin_.window.DialogControlElement.md)
- [WebviewViewResolveContext](../interfaces/cloudide_plugin_.window.WebviewViewResolveContext.md)

### Variables

- [activeColorTheme](cloudide_plugin_.window.md#activecolortheme)
- [activeTerminal](cloudide_plugin_.window.md#activeterminal)
- [activeTextEditor](cloudide_plugin_.window.md#activetexteditor)
- [state](cloudide_plugin_.window.md#state)
- [terminals](cloudide_plugin_.window.md#terminals)
- [visibleTextEditors](cloudide_plugin_.window.md#visibletexteditors)

### Functions

- [createCloudWebviewPanel](cloudide_plugin_.window.md#createcloudwebviewpanel)
- [createCustomizableDialog](cloudide_plugin_.window.md#createcustomizabledialog)
- [createInputBox](cloudide_plugin_.window.md#createinputbox)
- [createOutputChannel](cloudide_plugin_.window.md#createoutputchannel)
- [createQuickPick](cloudide_plugin_.window.md#createquickpick)
- [createStatusBarItem](cloudide_plugin_.window.md#createstatusbaritem)
- [createTerminal](cloudide_plugin_.window.md#createterminal)
- [createTextEditorDecorationType](cloudide_plugin_.window.md#createtexteditordecorationtype)
- [createTreeView](cloudide_plugin_.window.md#createtreeview)
- [createWebviewPanel](cloudide_plugin_.window.md#createwebviewpanel)
- [onDidChangeActiveColorTheme](cloudide_plugin_.window.md#ondidchangeactivecolortheme)
- [onDidChangeActiveTerminal](cloudide_plugin_.window.md#ondidchangeactiveterminal)
- [onDidChangeActiveTextEditor](cloudide_plugin_.window.md#ondidchangeactivetexteditor)
- [onDidChangeTextEditorOptions](cloudide_plugin_.window.md#ondidchangetexteditoroptions)
- [onDidChangeTextEditorSelection](cloudide_plugin_.window.md#ondidchangetexteditorselection)
- [onDidChangeTextEditorViewColumn](cloudide_plugin_.window.md#ondidchangetexteditorviewcolumn)
- [onDidChangeTextEditorVisibleRanges](cloudide_plugin_.window.md#ondidchangetexteditorvisibleranges)
- [onDidChangeVisibleTextEditors](cloudide_plugin_.window.md#ondidchangevisibletexteditors)
- [onDidChangeWindowState](cloudide_plugin_.window.md#ondidchangewindowstate)
- [onDidCloseTerminal](cloudide_plugin_.window.md#ondidcloseterminal)
- [onDidOpenTerminal](cloudide_plugin_.window.md#ondidopenterminal)
- [registerCustomEditorProvider](cloudide_plugin_.window.md#registercustomeditorprovider)
- [registerFileDecorationProvider](cloudide_plugin_.window.md#registerfiledecorationprovider)
- [registerTerminalLinkProvider](cloudide_plugin_.window.md#registerterminallinkprovider)
- [registerTreeDataProvider](cloudide_plugin_.window.md#registertreedataprovider)
- [registerUriHandler](cloudide_plugin_.window.md#registerurihandler)
- [registerWebviewAsPluginPage](cloudide_plugin_.window.md#registerwebviewaspluginpage)
- [registerWebviewPanelSerializer](cloudide_plugin_.window.md#registerwebviewpanelserializer)
- [registerWebviewViewProvider](cloudide_plugin_.window.md#registerwebviewviewprovider)
- [setStatusBarMessage](cloudide_plugin_.window.md#setstatusbarmessage)
- [showErrorMessage](cloudide_plugin_.window.md#showerrormessage)
- [showInformationMessage](cloudide_plugin_.window.md#showinformationmessage)
- [showInputBox](cloudide_plugin_.window.md#showinputbox)
- [showOpenDialog](cloudide_plugin_.window.md#showopendialog)
- [showQuickPick](cloudide_plugin_.window.md#showquickpick)
- [showSaveDialog](cloudide_plugin_.window.md#showsavedialog)
- [showTextDocument](cloudide_plugin_.window.md#showtextdocument)
- [showUploadDialog](cloudide_plugin_.window.md#showuploaddialog)
- [showWarningMessage](cloudide_plugin_.window.md#showwarningmessage)
- [showWorkspaceFolderPick](cloudide_plugin_.window.md#showworkspacefolderpick)
- [withProgress](cloudide_plugin_.window.md#withprogress)

## Variables

### activeColorTheme

• **activeColorTheme**: [`ColorTheme`](../interfaces/cloudide_plugin_.ColorTheme.md)

The currently active color theme as configured in the settings. The active
theme can be changed via the `workbench.colorTheme` setting.

#### Defined in

[index.d.ts:4893](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4893)

___

### activeTerminal

• **activeTerminal**: [`Terminal`](../interfaces/cloudide_plugin_.Terminal.md) \| `undefined`

The currently active terminal or undefined. The active terminal is the one
that currently has focus or most recently had focus.

#### Defined in

[index.d.ts:4132](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4132)

___

### activeTextEditor

• **activeTextEditor**: [`TextEditor`](../interfaces/cloudide_plugin_.TextEditor.md) \| `undefined`

The currently active editor or `undefined`. The active editor is the one
that currently has focus or, when none has focus, the one that has changed
input most recently.

#### Defined in

[index.d.ts:4139](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4139)

___

### state

• `Readonly` **state**: [`WindowState`](../interfaces/cloudide_plugin_.WindowState.md)

Represents the current window's state.

#### Defined in

[index.d.ts:4709](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4709)

___

### terminals

• **terminals**: `ReadonlyArray`<[`Terminal`](../interfaces/cloudide_plugin_.Terminal.md)\>

The currently opened terminals or an empty array.

#### Defined in

[index.d.ts:4144](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4144)

___

### visibleTextEditors

• **visibleTextEditors**: [`TextEditor`](../interfaces/cloudide_plugin_.TextEditor.md)[]

The currently visible editors or an empty array.

#### Defined in

[index.d.ts:4149](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4149)

## Functions

### createCloudWebviewPanel

▸ **createCloudWebviewPanel**(`viewType`, `title`, `showOptions`, `options?`): [`WebviewPanel`](../interfaces/cloudide_plugin_.WebviewPanel.md)

Create and show a new webview panel.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewType` | `string` | Identifies the type of the webview panel. |
| `title` | `string` | Title of the panel. |
| `showOptions` | [`ViewColumn`](../enums/cloudide_plugin_.ViewColumn.md) \| { `area`: `string` ; `preserveFocus?`: `boolean` ; `viewColumn`: [`ViewColumn`](../enums/cloudide_plugin_.ViewColumn.md)  } | where webview panel will be reside. If preserveFocus is set, the new webview will not take focus. |
| `options?` | [`WebviewPanelOptions`](../interfaces/cloudide_plugin_.WebviewPanelOptions.md) & [`WebviewOptions`](../interfaces/cloudide_plugin_.WebviewOptions.md) | Settings for the new panel. |

#### Returns

[`WebviewPanel`](../interfaces/cloudide_plugin_.WebviewPanel.md)

New webview panel.

#### Defined in

[index.d.ts:4581](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4581)

___

### createCustomizableDialog

▸ **createCustomizableDialog**(`options`): `Promise`<[`CustomizableDialog`](../interfaces/cloudide_plugin_.window.CustomizableDialog.md)\>

Create and open a dialog with an embedded iframe, it will allow you to:

- set the title of the dialog
- customize the width and height of the dialog
- set the content to any style
- control whether the close button is displayed
- control the content and alignment of the bottom button

It provides `onclose` callback triggered when the dialog is closed,
the callback parameters can be set to the data emited from dialog and the target element clicked when close dialog.

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`CustomizableDialogOptions`](../interfaces/cloudide_plugin_.window.CustomizableDialogOptions.md) |

#### Returns

`Promise`<[`CustomizableDialog`](../interfaces/cloudide_plugin_.window.CustomizableDialog.md)\>

CustomizableDialog

#### Defined in

[index.d.ts:4448](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4448)

___

### createInputBox

▸ **createInputBox**(): [`InputBox`](../interfaces/cloudide_plugin_.InputBox.md)

Creates a [InputBox](#InputBox) to let the user enter some text input.

Note that in many cases the more convenient [window.showInputBox](#window.showInputBox)
is easier to use. [window.createInputBox](#window.createInputBox) should be used
when [window.showInputBox](#window.showInputBox) does not offer the required flexibility.

#### Returns

[`InputBox`](../interfaces/cloudide_plugin_.InputBox.md)

A new [InputBox](#InputBox).

#### Defined in

[index.d.ts:4872](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4872)

___

### createOutputChannel

▸ **createOutputChannel**(`name`): [`OutputChannel`](../interfaces/cloudide_plugin_.OutputChannel.md)

Create a new [output channel](#OutputChannel) with the given name.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | String which will be used to represent the channel in the UI. |

#### Returns

[`OutputChannel`](../interfaces/cloudide_plugin_.OutputChannel.md)

#### Defined in

[index.d.ts:4765](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4765)

___

### createQuickPick

▸ **createQuickPick**<`T`\>(): [`QuickPick`](../interfaces/cloudide_plugin_.QuickPick.md)<`T`\>

Creates a [QuickPick](#QuickPick) to let the user pick an item from a list
of items of type T.

Note that in many cases the more convenient [window.showQuickPick](#window.showQuickPick)
is easier to use. [window.createQuickPick](#window.createQuickPick) should be used
when [window.showQuickPick](#window.showQuickPick) does not offer the required flexibility.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`QuickPickItem`](../interfaces/cloudide_plugin_.QuickPickItem.md) |

#### Returns

[`QuickPick`](../interfaces/cloudide_plugin_.QuickPick.md)<`T`\>

A new [QuickPick](#QuickPick).

#### Defined in

[index.d.ts:4267](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4267)

___

### createStatusBarItem

▸ **createStatusBarItem**(`alignment?`, `priority?`): [`StatusBarItem`](../interfaces/cloudide_plugin_.StatusBarItem.md)

Creates a status bar [item](#StatusBarItem).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `alignment?` | [`StatusBarAlignment`](../enums/cloudide_plugin_.StatusBarAlignment.md) | The alignment of the item. |
| `priority?` | `number` | The priority of the item. Higher values mean the item should be shown more to the left. |

#### Returns

[`StatusBarItem`](../interfaces/cloudide_plugin_.StatusBarItem.md)

A new status bar item.

#### Defined in

[index.d.ts:4758](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4758)

___

### createTerminal

▸ **createTerminal**(`name?`, `shellPath?`, `shellArgs?`): [`Terminal`](../interfaces/cloudide_plugin_.Terminal.md)

Create new terminal.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name?` | `string` | terminal name to display on the UI. |
| `shellPath?` | `string` | path to the executable shell. For example "/bin/bash", "bash", "sh". |
| `shellArgs?` | `string`[] | arguments to configure executable shell. For example ["-l"] - run shell without login. |

#### Returns

[`Terminal`](../interfaces/cloudide_plugin_.Terminal.md)

#### Defined in

[index.d.ts:4773](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4773)

▸ **createTerminal**(`options`): [`Terminal`](../interfaces/cloudide_plugin_.Terminal.md)

Create new terminal with predefined options.

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`TerminalOptions`](../interfaces/cloudide_plugin_.TerminalOptions.md) |

#### Returns

[`Terminal`](../interfaces/cloudide_plugin_.Terminal.md)

#### Defined in

[index.d.ts:4790](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4790)

▸ **createTerminal**(`options`): [`Terminal`](../interfaces/cloudide_plugin_.Terminal.md)

Creates a pseudo where an extension controls its input and output.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`PseudoTerminalOptions`](../interfaces/cloudide_plugin_.PseudoTerminalOptions.md) | PseudoTerminalOptions. |

#### Returns

[`Terminal`](../interfaces/cloudide_plugin_.Terminal.md)

A new Terminal.

#### Defined in

[index.d.ts:4798](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4798)

___

### createTextEditorDecorationType

▸ **createTextEditorDecorationType**(`options`): [`TextEditorDecorationType`](../interfaces/cloudide_plugin_.TextEditorDecorationType.md)

Create a TextEditorDecorationType that can be used to add decorations to text editors.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`DecorationRenderOptions`](../interfaces/cloudide_plugin_.DecorationRenderOptions.md) | Rendering options for the decoration type. |

#### Returns

[`TextEditorDecorationType`](../interfaces/cloudide_plugin_.TextEditorDecorationType.md)

A new decoration type instance.

#### Defined in

[index.d.ts:4723](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4723)

___

### createTreeView

▸ **createTreeView**<`T`\>(`viewId`, `options`): [`TreeView`](../interfaces/cloudide_plugin_.TreeView.md)<`T`\>

Create a [TreeView](#TreeView) for the view contributed using the extension point `views`.

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewId` | `string` | Id of the view contributed using the extension point `views`. |
| `options` | [`TreeViewOptions`](../interfaces/cloudide_plugin_.TreeViewOptions.md)<`T`\> | Options object to provide [TreeDataProvider](#TreeDataProvider) for the view. |

#### Returns

[`TreeView`](../interfaces/cloudide_plugin_.TreeView.md)<`T`\>

a [TreeView](#TreeView).

#### Defined in

[index.d.ts:4817](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4817)

___

### createWebviewPanel

▸ **createWebviewPanel**(`viewType`, `title`, `showOptions`, `options?`): [`WebviewPanel`](../interfaces/cloudide_plugin_.WebviewPanel.md)

Create and show a new webview panel.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewType` | `string` | Identifies the type of the webview panel. |
| `title` | `string` | Title of the panel. |
| `showOptions` | [`ViewColumn`](../enums/cloudide_plugin_.ViewColumn.md) \| [`WebviewPanelShowOptions`](../interfaces/cloudide_plugin_.WebviewPanelShowOptions.md) | where webview panel will be reside. If preserveFocus is set, the new webview will not take focus. |
| `options?` | [`WebviewPanelOptions`](../interfaces/cloudide_plugin_.WebviewPanelOptions.md) & [`WebviewOptions`](../interfaces/cloudide_plugin_.WebviewOptions.md) | Settings for the new panel. |

#### Returns

[`WebviewPanel`](../interfaces/cloudide_plugin_.WebviewPanel.md)

New webview panel.

#### Defined in

[index.d.ts:4568](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4568)

___

### onDidChangeActiveColorTheme

▸ **onDidChangeActiveColorTheme**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`ColorTheme`](../interfaces/cloudide_plugin_.ColorTheme.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidChangeActiveTerminal

▸ **onDidChangeActiveTerminal**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: `undefined` \| [`Terminal`](../interfaces/cloudide_plugin_.Terminal.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidChangeActiveTextEditor

▸ **onDidChangeActiveTextEditor**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: `undefined` \| [`TextEditor`](../interfaces/cloudide_plugin_.TextEditor.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidChangeTextEditorOptions

▸ **onDidChangeTextEditorOptions**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TextEditorOptionsChangeEvent`](../interfaces/cloudide_plugin_.TextEditorOptionsChangeEvent.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidChangeTextEditorSelection

▸ **onDidChangeTextEditorSelection**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TextEditorSelectionChangeEvent`](../interfaces/cloudide_plugin_.TextEditorSelectionChangeEvent.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidChangeTextEditorViewColumn

▸ **onDidChangeTextEditorViewColumn**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TextEditorViewColumnChangeEvent`](../interfaces/cloudide_plugin_.TextEditorViewColumnChangeEvent.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidChangeTextEditorVisibleRanges

▸ **onDidChangeTextEditorVisibleRanges**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TextEditorVisibleRangesChangeEvent`](../interfaces/cloudide_plugin_.TextEditorVisibleRangesChangeEvent.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidChangeVisibleTextEditors

▸ **onDidChangeVisibleTextEditors**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TextEditor`](../interfaces/cloudide_plugin_.TextEditor.md)[]) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidChangeWindowState

▸ **onDidChangeWindowState**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`WindowState`](../interfaces/cloudide_plugin_.WindowState.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidCloseTerminal

▸ **onDidCloseTerminal**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`Terminal`](../interfaces/cloudide_plugin_.Terminal.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidOpenTerminal

▸ **onDidOpenTerminal**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`Terminal`](../interfaces/cloudide_plugin_.Terminal.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### registerCustomEditorProvider

▸ **registerCustomEditorProvider**(`viewType`, `provider`, `options?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a provider for custom editors for the `viewType` contributed by the `customEditors` extension point.

When a custom editor is opened, Theia fires an `onCustomEditor:viewType` activation event. Your extension
must register a [`CustomTextEditorProvider`](#CustomTextEditorProvider), [`CustomReadonlyEditorProvider`](#CustomReadonlyEditorProvider),
[`CustomEditorProvider`](#CustomEditorProvider)for `viewType` as part of activation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewType` | `string` | Unique identifier for the custom editor provider. This should match the `viewType` from the `customEditors` contribution point. |
| `provider` | [`CustomTextEditorProvider`](../interfaces/cloudide_plugin_.CustomTextEditorProvider.md) \| [`CustomReadonlyEditorProvider`](../interfaces/cloudide_plugin_.CustomReadonlyEditorProvider.md)<[`CustomDocument`](../interfaces/cloudide_plugin_.CustomDocument.md)\> \| [`CustomEditorProvider`](../interfaces/cloudide_plugin_.CustomEditorProvider.md)<[`CustomDocument`](../interfaces/cloudide_plugin_.CustomDocument.md)\> | Provider that resolves custom editors. |
| `options?` | `Object` | Options for the provider. |
| `options.supportsMultipleEditorsPerDocument?` | `boolean` | Only applies to `CustomReadonlyEditorProvider \| CustomEditorProvider`. Indicates that the provider allows multiple editor instances to be open at the same time for the same resource. By default, Theia only allows one editor instance to be open at a time for each resource. If the user tries to open a second editor instance for the resource, the first one is instead moved to where the second one was to be opened. When `supportsMultipleEditorsPerDocument` is enabled, users can split and create copies of the custom editor. In this case, the custom editor must make sure it can properly synchronize the states of all editor instances for a resource so that they are consistent. |
| `options.webviewOptions?` | [`WebviewPanelOptions`](../interfaces/cloudide_plugin_.WebviewPanelOptions.md) | Content settings for the webview panels created for this custom editor. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Disposable that unregisters the provider.

#### Defined in

[index.d.ts:4681](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4681)

___

### registerFileDecorationProvider

▸ **registerFileDecorationProvider**(`provider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a file decoration provider.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `provider` | [`FileDecorationProvider`](../interfaces/cloudide_plugin_.FileDecorationProvider.md) | A [FileDecorationProvider](#FileDecorationProvider). |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters the provider.

#### Defined in

[index.d.ts:4887](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4887)

___

### registerTerminalLinkProvider

▸ **registerTerminalLinkProvider**(`provider`): `void`

Register provider that enables the detection and handling of links within the terminal.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `provider` | [`TerminalLinkProvider`](../interfaces/cloudide_plugin_.TerminalLinkProvider.md)<[`TerminalLink`](../interfaces/cloudide_plugin_.TerminalLink.md)\> | The provider that provides the terminal links. |

#### Returns

`void`

Disposable that unregisters the provider.

#### Defined in

[index.d.ts:4879](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4879)

___

### registerTreeDataProvider

▸ **registerTreeDataProvider**<`T`\>(`viewId`, `treeDataProvider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a [TreeDataProvider](#TreeDataProvider) for the view contributed using the extension point `views`.
This will allow you to contribute data to the [TreeView](#TreeView) and update if the data changes.

**Note:** To get access to the [TreeView](#TreeView) and perform operations on it, use [createTreeView](#window.createTreeView).

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewId` | `string` | Id of the view contributed using the extension point `views`. |
| `treeDataProvider` | [`TreeDataProvider`](../interfaces/cloudide_plugin_.TreeDataProvider.md)<`T`\> | A [TreeDataProvider](#TreeDataProvider) that provides tree data for the view |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Defined in

[index.d.ts:4809](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4809)

___

### registerUriHandler

▸ **registerUriHandler**(`handler`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Registers a [uri handler](#UriHandler) capable of handling system-wide [uris](#Uri).
In case there are multiple windows open, the topmost window will handle the uri.
A uri handler is scoped to the extension it is contributed from; it will only
be able to handle uris which are directed to the extension itself. A uri must respect
the following rules:

- The uri-scheme must be the product name;
- The uri-authority must be the extension id (eg. `my.extension`);
- The uri-path, -query and -fragment parts are arbitrary.

For example, if the `my.extension` extension registers a uri handler, it will only
be allowed to handle uris with the prefix `product-name://my.extension`.

An extension can only register a single uri handler in its entire activation lifetime.

* *Note:* There is an activation event `onUri` that fires when a uri directed for
the current extension is about to be handled.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `handler` | [`UriHandler`](../interfaces/cloudide_plugin_.UriHandler.md) | The uri handler to register for this extension. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Defined in

[index.d.ts:4840](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4840)

___

### registerWebviewAsPluginPage

▸ **registerWebviewAsPluginPage**(`viewType`): `void`

Only registers a webview panel.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewType` | `string` | Type of the webview panel. |

#### Returns

`void`

#### Defined in

[index.d.ts:4665](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4665)

___

### registerWebviewPanelSerializer

▸ **registerWebviewPanelSerializer**(`viewType`, `serializer`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `viewType` | `string` |
| `serializer` | [`WebviewPanelSerializer`](../interfaces/cloudide_plugin_.WebviewPanelSerializer.md)<`unknown`\> |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Defined in

[index.d.ts:4658](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4658)

___

### registerWebviewViewProvider

▸ **registerWebviewViewProvider**(`viewId`, `provider`, `options?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewId` | `string` | - |
| `provider` | [`WebviewViewProvider`](../interfaces/cloudide_plugin_.WebviewViewProvider.md) | - |
| `options?` | `Object` | - |
| `options.webviewOptions?` | `Object` | Content settings for the webview created for this view. |
| `options.webviewOptions.retainContextWhenHidden?` | `boolean` | Controls if the webview element itself (iframe) is kept around even when the view is no longer visible. Normally the webview's html context is created when the view becomes visible and destroyed when it is hidden. Extensions that have complex state or UI can set the `retainContextWhenHidden` to make the editor keep the webview context around, even when the webview moves to a background tab. When a webview using `retainContextWhenHidden` becomes hidden, its scripts and other dynamic content are suspended. When the view becomes visible again, the context is automatically restored in the exact same state it was in originally. You cannot send messages to a hidden webview, even with `retainContextWhenHidden` enabled. `retainContextWhenHidden` has a high memory overhead and should only be used if your view's context cannot be quickly saved and restored. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Defined in

[index.d.ts:4633](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4633)

___

### setStatusBarMessage

▸ **setStatusBarMessage**(`text`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Set a message to the status bar.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` | The message to show, supports icon substitution as in status bar. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A disposable which hides the status bar message.

#### Defined in

[index.d.ts:4731](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4731)

▸ **setStatusBarMessage**(`text`, `hideAfterTimeout`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Set a message to the status bar.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` | The message to show, supports icon substitution as in status bar. |
| `hideAfterTimeout` | `number` | Timeout in milliseconds after which the message will be disposed. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A disposable which hides the status bar message.

#### Defined in

[index.d.ts:4740](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4740)

▸ **setStatusBarMessage**(`text`, `hideWhenDone`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Set a message to the status bar.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` | The message to show, supports icon substitution as in status bar. |
| `hideWhenDone` | `PromiseLike`<`any`\> | PromiseLike on which completion (resolve or reject) the message will be disposed. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A disposable which hides the status bar message.

#### Defined in

[index.d.ts:4749](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4749)

___

### showErrorMessage

▸ **showErrorMessage**(`message`, `...items`): `PromiseLike`<`string` \| `undefined`\>

Show an error message.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | a message to show. |
| `...items` | `string`[] | A set of items that will be rendered as actions in the message. |

#### Returns

`PromiseLike`<`string` \| `undefined`\>

A promise that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:4361](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4361)

▸ **showErrorMessage**(`message`, `options`, `...items`): `PromiseLike`<`string` \| `undefined`\>

Show an error message.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | a message to show. |
| `options` | [`MessageOptions`](../interfaces/cloudide_plugin_.MessageOptions.md) | Configures the behaviour of the message. |
| `...items` | `string`[] | A set of items that will be rendered as actions in the message. |

#### Returns

`PromiseLike`<`string` \| `undefined`\>

A promise that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:4371](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4371)

▸ **showErrorMessage**<`T`\>(`message`, `...items`): `PromiseLike`<`T` \| `undefined`\>

Show an error message.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`MessageItem`](../interfaces/cloudide_plugin_.MessageItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | a message to show. |
| `...items` | `T`[] | A set of items that will be rendered as actions in the message. |

#### Returns

`PromiseLike`<`T` \| `undefined`\>

A promise that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:4380](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4380)

▸ **showErrorMessage**<`T`\>(`message`, `options`, `...items`): `PromiseLike`<`T` \| `undefined`\>

Show an error message.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`MessageItem`](../interfaces/cloudide_plugin_.MessageItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | a message to show. |
| `options` | [`MessageOptions`](../interfaces/cloudide_plugin_.MessageOptions.md) | Configures the behaviour of the message. |
| `...items` | `T`[] | A set of items that will be rendered as actions in the message. |

#### Returns

`PromiseLike`<`T` \| `undefined`\>

A promise that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:4390](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4390)

___

### showInformationMessage

▸ **showInformationMessage**(`message`, `...items`): `PromiseLike`<`string` \| `undefined`\>

Show an information message.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | a message to show. |
| `...items` | `string`[] | A set of items that will be rendered as actions in the message. |

#### Returns

`PromiseLike`<`string` \| `undefined`\>

A promise that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:4285](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4285)

▸ **showInformationMessage**(`message`, `options`, `...items`): `PromiseLike`<`string` \| `undefined`\>

Show an information message.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | a message to show. |
| `options` | [`MessageOptions`](../interfaces/cloudide_plugin_.MessageOptions.md) | Configures the behaviour of the message. |
| `...items` | `string`[] | A set of items that will be rendered as actions in the message. |

#### Returns

`PromiseLike`<`string` \| `undefined`\>

A promise that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:4295](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4295)

▸ **showInformationMessage**<`T`\>(`message`, `...items`): `PromiseLike`<`T` \| `undefined`\>

Show an information message.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`MessageItem`](../interfaces/cloudide_plugin_.MessageItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | a message to show. |
| `...items` | `T`[] | A set of items that will be rendered as actions in the message. |

#### Returns

`PromiseLike`<`T` \| `undefined`\>

A promise that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:4304](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4304)

▸ **showInformationMessage**<`T`\>(`message`, `options`, `...items`): `PromiseLike`<`T` \| `undefined`\>

Show an information message.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`MessageItem`](../interfaces/cloudide_plugin_.MessageItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | a message to show. |
| `options` | [`MessageOptions`](../interfaces/cloudide_plugin_.MessageOptions.md) | Configures the behaviour of the message. |
| `...items` | `T`[] | A set of items that will be rendered as actions in the message. |

#### Returns

`PromiseLike`<`T` \| `undefined`\>

A promise that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:4314](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4314)

___

### showInputBox

▸ **showInputBox**(`options?`, `token?`): `PromiseLike`<`string` \| `undefined`\>

Opens an input box to ask the user for input.

The returned value will be `undefined` if the input box was canceled (e.g. pressing ESC). Otherwise the
returned value will be the string typed by the user or an empty string if the user did not type
anything but dismissed the input box with OK.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | [`InputBoxOptions`](../interfaces/cloudide_plugin_.InputBoxOptions.md) | Configures the behavior of the input box. |
| `token?` | [`CancellationToken`](../interfaces/cloudide_plugin_.CancellationToken.md) | A token that can be used to signal cancellation. |

#### Returns

`PromiseLike`<`string` \| `undefined`\>

A promise that resolves to a string the user provided or to `undefined` in case of dismissal.

#### Defined in

[index.d.ts:4403](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4403)

___

### showOpenDialog

▸ **showOpenDialog**(`options`): `PromiseLike`<[`Uri`](../classes/cloudide_plugin_.Uri.md)[] \| `undefined`\>

Shows a file open dialog to the user which allows to select a file
for opening-purposes.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`OpenDialogOptions`](../interfaces/cloudide_plugin_.OpenDialogOptions.md) | Options that control the dialog. |

#### Returns

`PromiseLike`<[`Uri`](../classes/cloudide_plugin_.Uri.md)[] \| `undefined`\>

A promise that resolves to the selected resources or `undefined`.

#### Defined in

[index.d.ts:4412](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4412)

___

### showQuickPick

▸ **showQuickPick**(`items`, `options`, `token?`): `PromiseLike`<`string` \| `undefined`\>

Shows a selection list.

#### Parameters

| Name | Type |
| :------ | :------ |
| `items` | `string`[] \| `PromiseLike`<`string`[]\> |
| `options` | [`QuickPickOptions`](../interfaces/cloudide_plugin_.QuickPickOptions.md) |
| `token?` | [`CancellationToken`](../interfaces/cloudide_plugin_.CancellationToken.md) |

#### Returns

`PromiseLike`<`string` \| `undefined`\>

#### Defined in

[index.d.ts:4230](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4230)

▸ **showQuickPick**(`items`, `options`, `token?`): `PromiseLike`<`string`[] \| `undefined`\>

Shows a selection list with multiple selection allowed.

#### Parameters

| Name | Type |
| :------ | :------ |
| `items` | `string`[] \| `PromiseLike`<`string`[]\> |
| `options` | [`QuickPickOptions`](../interfaces/cloudide_plugin_.QuickPickOptions.md) & { `canPickMany`: ``true``  } |
| `token?` | [`CancellationToken`](../interfaces/cloudide_plugin_.CancellationToken.md) |

#### Returns

`PromiseLike`<`string`[] \| `undefined`\>

#### Defined in

[index.d.ts:4235](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4235)

▸ **showQuickPick**<`T`\>(`items`, `options`, `token?`): `PromiseLike`<`T` \| `undefined`\>

Shows a selection list.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`QuickPickItem`](../interfaces/cloudide_plugin_.QuickPickItem.md) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `items` | `T`[] \| `PromiseLike`<`T`[]\> |
| `options` | [`QuickPickOptions`](../interfaces/cloudide_plugin_.QuickPickOptions.md) |
| `token?` | [`CancellationToken`](../interfaces/cloudide_plugin_.CancellationToken.md) |

#### Returns

`PromiseLike`<`T` \| `undefined`\>

#### Defined in

[index.d.ts:4247](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4247)

▸ **showQuickPick**<`T`\>(`items`, `options`, `token?`): `PromiseLike`<`T`[] \| `undefined`\>

Shows a selection list with multiple selection allowed.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`QuickPickItem`](../interfaces/cloudide_plugin_.QuickPickItem.md) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `items` | `T`[] \| `PromiseLike`<`T`[]\> |
| `options` | [`QuickPickOptions`](../interfaces/cloudide_plugin_.QuickPickOptions.md) & { `canPickMany`: ``true``  } |
| `token?` | [`CancellationToken`](../interfaces/cloudide_plugin_.CancellationToken.md) |

#### Returns

`PromiseLike`<`T`[] \| `undefined`\>

#### Defined in

[index.d.ts:4252](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4252)

___

### showSaveDialog

▸ **showSaveDialog**(`options`): `PromiseLike`<[`Uri`](../classes/cloudide_plugin_.Uri.md) \| `undefined`\>

Shows a file save dialog to the user which allows to select a file
for saving-purposes.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`SaveDialogOptions`](../interfaces/cloudide_plugin_.SaveDialogOptions.md) | Options that control the dialog. |

#### Returns

`PromiseLike`<[`Uri`](../classes/cloudide_plugin_.Uri.md) \| `undefined`\>

A promise that resolves to the selected resource or `undefined`.

#### Defined in

[index.d.ts:4421](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4421)

___

### showTextDocument

▸ **showTextDocument**(`document`, `column?`, `preserveFocus?`): `PromiseLike`<[`TextEditor`](../interfaces/cloudide_plugin_.TextEditor.md)\>

Show the given document in a text editor. A [column](#ViewColumn) can be provided
to control where the editor is being shown. Might change the [active editor](#window.activeTextEditor).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](../interfaces/cloudide_plugin_.TextDocument.md) | A text document to be shown. |
| `column?` | [`ViewColumn`](../enums/cloudide_plugin_.ViewColumn.md) | A view column in which the [editor](#TextEditor) should be shown. The default is the [active](#ViewColumn.Active), other values are adjusted to be `Min(column, columnCount + 1)`, the [active](#ViewColumn.Active)-column is not adjusted. Use [`ViewColumn.Beside`](#ViewColumn.Beside) to open the editor to the side of the currently active one. |
| `preserveFocus?` | `boolean` | When `true` the editor will not take focus. |

#### Returns

`PromiseLike`<[`TextEditor`](../interfaces/cloudide_plugin_.TextEditor.md)\>

A promise that resolves to an [editor](#TextEditor).

#### Defined in

[index.d.ts:4201](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4201)

▸ **showTextDocument**(`document`, `options?`): `PromiseLike`<[`TextEditor`](../interfaces/cloudide_plugin_.TextEditor.md)\>

Show the given document in a text editor. [Options](#TextDocumentShowOptions) can be provided
to control options of the editor is being shown. Might change the [active editor](#window.activeTextEditor).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](../interfaces/cloudide_plugin_.TextDocument.md) | A text document to be shown. |
| `options?` | [`TextDocumentShowOptions`](../interfaces/cloudide_plugin_.TextDocumentShowOptions.md) | [Editor options](#TextDocumentShowOptions) to configure the behavior of showing the [editor](#TextEditor). |

#### Returns

`PromiseLike`<[`TextEditor`](../interfaces/cloudide_plugin_.TextEditor.md)\>

A promise that resolves to an [editor](#TextEditor).

#### Defined in

[index.d.ts:4211](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4211)

▸ **showTextDocument**(`uri`, `options?`): `PromiseLike`<[`TextEditor`](../interfaces/cloudide_plugin_.TextEditor.md)\>

A short-hand for `openTextDocument(uri).then(document => showTextDocument(document, options))`.

**`See`**

[openTextDocument](#openTextDocument)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | A resource identifier. |
| `options?` | [`TextDocumentShowOptions`](../interfaces/cloudide_plugin_.TextDocumentShowOptions.md) | [Editor options](#TextDocumentShowOptions) to configure the behavior of showing the [editor](#TextEditor). |

#### Returns

`PromiseLike`<[`TextEditor`](../interfaces/cloudide_plugin_.TextEditor.md)\>

A promise that resolves to an [editor](#TextEditor).

#### Defined in

[index.d.ts:4222](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4222)

___

### showUploadDialog

▸ **showUploadDialog**(`options`): `PromiseLike`<[`Uri`](../classes/cloudide_plugin_.Uri.md)[] \| `undefined`\>

Shows a file upload dialog to the user which allows to upload files
for various purposes.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`UploadDialogOptions`](../interfaces/cloudide_plugin_.UploadDialogOptions.md) | Options, that control the dialog. |

#### Returns

`PromiseLike`<[`Uri`](../classes/cloudide_plugin_.Uri.md)[] \| `undefined`\>

A promise that resolves the paths of uploaded files or `undefined`.

#### Defined in

[index.d.ts:4430](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4430)

___

### showWarningMessage

▸ **showWarningMessage**(`message`, `...items`): `PromiseLike`<`string` \| `undefined`\>

Show a warning message.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | a message to show. |
| `...items` | `string`[] | A set of items that will be rendered as actions in the message. |

#### Returns

`PromiseLike`<`string` \| `undefined`\>

A promise that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:4323](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4323)

▸ **showWarningMessage**(`message`, `options`, `...items`): `PromiseLike`<`string` \| `undefined`\>

Show a warning message.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | a message to show. |
| `options` | [`MessageOptions`](../interfaces/cloudide_plugin_.MessageOptions.md) | Configures the behaviour of the message. |
| `...items` | `string`[] | A set of items that will be rendered as actions in the message. |

#### Returns

`PromiseLike`<`string` \| `undefined`\>

A promise that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:4333](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4333)

▸ **showWarningMessage**<`T`\>(`message`, `...items`): `PromiseLike`<`T` \| `undefined`\>

Show a warning message.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`MessageItem`](../interfaces/cloudide_plugin_.MessageItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | a message to show. |
| `...items` | `T`[] | A set of items that will be rendered as actions in the message. |

#### Returns

`PromiseLike`<`T` \| `undefined`\>

A promise that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:4342](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4342)

▸ **showWarningMessage**<`T`\>(`message`, `options`, `...items`): `PromiseLike`<`T` \| `undefined`\>

Show a warning message.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`MessageItem`](../interfaces/cloudide_plugin_.MessageItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | a message to show. |
| `options` | [`MessageOptions`](../interfaces/cloudide_plugin_.MessageOptions.md) | Configures the behaviour of the message. |
| `...items` | `T`[] | A set of items that will be rendered as actions in the message. |

#### Returns

`PromiseLike`<`T` \| `undefined`\>

A promise that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:4352](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4352)

___

### showWorkspaceFolderPick

▸ **showWorkspaceFolderPick**(`options?`): `PromiseLike`<[`WorkspaceFolder`](../interfaces/cloudide_plugin_.WorkspaceFolder.md) \| `undefined`\>

Shows a selection list of [workspace folders](#workspace.workspaceFolders) to pick from.
Returns `undefined` if no folder is open.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | [`WorkspaceFolderPickOptions`](../interfaces/cloudide_plugin_.WorkspaceFolderPickOptions.md) | Configures the behavior of the workspace folder list. |

#### Returns

`PromiseLike`<[`WorkspaceFolder`](../interfaces/cloudide_plugin_.WorkspaceFolder.md) \| `undefined`\>

A promise that resolves to the workspace folder or `undefined`.

#### Defined in

[index.d.ts:4276](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4276)

___

### withProgress

▸ **withProgress**<`R`\>(`options`, `task`): `PromiseLike`<`R`\>

Show progress in the editor. Progress is shown while running the given callback
and while the promise it returned isn't resolved nor rejected. The location at which
progress should show (and other details) is defined via the passed [`ProgressOptions`](#ProgressOptions).

#### Type parameters

| Name |
| :------ |
| `R` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`ProgressOptions`](../interfaces/cloudide_plugin_.ProgressOptions.md) | - |
| `task` | (`progress`: [`Progress`](../interfaces/cloudide_plugin_.Progress.md)<{ `increment?`: `number` ; `message?`: `string`  }\>, `token`: [`CancellationToken`](../interfaces/cloudide_plugin_.CancellationToken.md)) => `PromiseLike`<`R`\> | A callback returning a promise. Progress state can be reported with the provided [progress](#Progress)-object. To report discrete progress, use `increment` to indicate how much work has been completed. Each call with a `increment` value will be summed up and reflected as overall progress until 100% is reached (a value of e.g. `10` accounts for `10%` of work done). Note that currently only `ProgressLocation.Notification` is capable of showing discrete progress. To monitor if the operation has been cancelled by the user, use the provided [`CancellationToken`](#CancellationToken). Note that currently only `ProgressLocation.Notification` is supporting to show a cancel button to cancel the long running operation. |

#### Returns

`PromiseLike`<`R`\>

The thenable the task-callback returned.

#### Defined in

[index.d.ts:4861](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4861)
