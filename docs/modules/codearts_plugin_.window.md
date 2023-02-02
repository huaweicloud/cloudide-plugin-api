[@codearts/plugin](../README.md) / ["@codearts/plugin"](_codearts_plugin_.md) / window

# Namespace: window

["@codearts/plugin"](_codearts_plugin_.md).window

Namespace for dealing with the current window of the editor. That is visible
and active editors, as well as, UI elements to show messages, selections, and
asking for user input.

## Table of contents

### Variables

- [activeColorTheme](codearts_plugin_.window.md#activecolortheme)
- [activeNotebookEditor](codearts_plugin_.window.md#activenotebookeditor)
- [activeTerminal](codearts_plugin_.window.md#activeterminal)
- [activeTextEditor](codearts_plugin_.window.md#activetexteditor)
- [selectedResources](codearts_plugin_.window.md#selectedresources)
- [state](codearts_plugin_.window.md#state)
- [tabGroups](codearts_plugin_.window.md#tabgroups)
- [terminals](codearts_plugin_.window.md#terminals)
- [visibleNotebookEditors](codearts_plugin_.window.md#visiblenotebookeditors)
- [visibleTextEditors](codearts_plugin_.window.md#visibletexteditors)

### Functions

- [createCloudWebviewPanel](codearts_plugin_.window.md#createcloudwebviewpanel)
- [createInputBox](codearts_plugin_.window.md#createinputbox)
- [createLightWebviewPanel](codearts_plugin_.window.md#createlightwebviewpanel)
- [createOutputChannel](codearts_plugin_.window.md#createoutputchannel)
- [createQuickPick](codearts_plugin_.window.md#createquickpick)
- [createStatusBarItem](codearts_plugin_.window.md#createstatusbaritem)
- [createTerminal](codearts_plugin_.window.md#createterminal)
- [createTextEditorDecorationType](codearts_plugin_.window.md#createtexteditordecorationtype)
- [createTreeView](codearts_plugin_.window.md#createtreeview)
- [createWebviewPanel](codearts_plugin_.window.md#createwebviewpanel)
- [createWebviewViewDialog](codearts_plugin_.window.md#createwebviewviewdialog)
- [getTerminalById](codearts_plugin_.window.md#getterminalbyid)
- [onDidChangeActiveColorTheme](codearts_plugin_.window.md#ondidchangeactivecolortheme)
- [onDidChangeActiveNotebookEditor](codearts_plugin_.window.md#ondidchangeactivenotebookeditor)
- [onDidChangeActiveTerminal](codearts_plugin_.window.md#ondidchangeactiveterminal)
- [onDidChangeActiveTextEditor](codearts_plugin_.window.md#ondidchangeactivetexteditor)
- [onDidChangeNotebookEditorSelection](codearts_plugin_.window.md#ondidchangenotebookeditorselection)
- [onDidChangeNotebookEditorVisibleRanges](codearts_plugin_.window.md#ondidchangenotebookeditorvisibleranges)
- [onDidChangeTerminalColor](codearts_plugin_.window.md#ondidchangeterminalcolor)
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
- [onDidRenameTerminal](codearts_plugin_.window.md#ondidrenameterminal)
- [registerComponentsInEditorGutter](codearts_plugin_.window.md#registercomponentsineditorgutter)
- [registerCustomEditorProvider](codearts_plugin_.window.md#registercustomeditorprovider)
- [registerFileDecorationProvider](codearts_plugin_.window.md#registerfiledecorationprovider)
- [registerMainMenu](codearts_plugin_.window.md#registermainmenu)
- [registerMenu](codearts_plugin_.window.md#registermenu)
- [registerMenuId](codearts_plugin_.window.md#registermenuid)
- [registerProjectWizardProvider](codearts_plugin_.window.md#registerprojectwizardprovider)
- [registerTerminalLinkProvider](codearts_plugin_.window.md#registerterminallinkprovider)
- [registerTerminalProfileProvider](codearts_plugin_.window.md#registerterminalprofileprovider)
- [registerTreeDataProvider](codearts_plugin_.window.md#registertreedataprovider)
- [registerUriHandler](codearts_plugin_.window.md#registerurihandler)
- [registerViewContainerSubTitle](codearts_plugin_.window.md#registerviewcontainersubtitle)
- [registerViewTitleActions](codearts_plugin_.window.md#registerviewtitleactions)
- [registerWebviewPanelSerializer](codearts_plugin_.window.md#registerwebviewpanelserializer)
- [registerWebviewViewProvider](codearts_plugin_.window.md#registerwebviewviewprovider)
- [setStatusBarMessage](codearts_plugin_.window.md#setstatusbarmessage)
- [showCodeTip](codearts_plugin_.window.md#showcodetip)
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
- [unregisterMainMenu](codearts_plugin_.window.md#unregistermainmenu)
- [unregisterMenu](codearts_plugin_.window.md#unregistermenu)
- [withProgress](codearts_plugin_.window.md#withprogress)
- [withScmProgress](codearts_plugin_.window.md#withscmprogress)

## Variables

### activeColorTheme

• **activeColorTheme**: [`ColorTheme`](../interfaces/codearts_plugin_.ColorTheme.md)

The currently active color theme as configured in the settings. The active
theme can be changed via the `workbench.colorTheme` setting.

#### Defined in

[index.d.ts:10354](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10354)

___

### activeNotebookEditor

• `Const` **activeNotebookEditor**: [`NotebookEditor`](../interfaces/codearts_plugin_.NotebookEditor.md) \| `undefined`

The currently active [notebook editor](../interfaces/codearts_plugin_.NotebookEditor.md) or `undefined`. The active editor is the one
that currently has focus or, when none has focus, the one that has changed
input most recently.

#### Defined in

[index.d.ts:9652](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9652)

___

### activeTerminal

• `Const` **activeTerminal**: [`Terminal`](../interfaces/codearts_plugin_.Terminal.md) \| `undefined`

The currently active terminal or `undefined`. The active terminal is the one that
currently has focus or most recently had focus.

#### Defined in

[index.d.ts:9682](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9682)

___

### activeTextEditor

• **activeTextEditor**: [`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md) \| `undefined`

The currently active editor or `undefined`. The active editor is the one
that currently has focus or, when none has focus, the one that has changed
input most recently.

#### Defined in

[index.d.ts:9596](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9596)

___

### selectedResources

• `Const` **selectedResources**: [`Uri`](../classes/codearts_plugin_.Uri.md)[]

An array of resource uri which are selected in explorer.

#### Defined in

[index.d.ts:10422](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10422)

___

### state

• `Const` **state**: [`WindowState`](../interfaces/codearts_plugin_.WindowState.md)

Represents the current window's state.

#### Defined in

[index.d.ts:9720](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9720)

___

### tabGroups

• `Const` **tabGroups**: [`TabGroups`](../interfaces/codearts_plugin_.TabGroups.md)

Represents the grid widget within the main editor area

#### Defined in

[index.d.ts:9589](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9589)

___

### terminals

• `Const` **terminals**: readonly [`Terminal`](../interfaces/codearts_plugin_.Terminal.md)[]

The currently opened terminals or an empty array.

#### Defined in

[index.d.ts:9676](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9676)

___

### visibleNotebookEditors

• `Const` **visibleNotebookEditors**: readonly [`NotebookEditor`](../interfaces/codearts_plugin_.NotebookEditor.md)[]

The currently visible [notebook editors](../interfaces/codearts_plugin_.NotebookEditor.md) or an empty array.

#### Defined in

[index.d.ts:9639](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9639)

___

### visibleTextEditors

• **visibleTextEditors**: readonly [`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)[]

The currently visible editors or an empty array.

#### Defined in

[index.d.ts:9601](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9601)

## Functions

### createCloudWebviewPanel

▸ **createCloudWebviewPanel**(`viewType`, `title`, `showOptions`, `options?`): [`WebviewContainer`](../interfaces/codearts_plugin_.WebviewContainer.md)

CreateCloudWebviewPanel is the same as createLightWebviewPanel, used in cloudide plugins.

**`Deprecated`**

Please use `createLightWebviewPanel`.

#### Parameters

| Name | Type |
| :------ | :------ |
| `viewType` | `string` |
| `title` | `string` |
| `showOptions` | [`WebviewShowOptions`](../interfaces/codearts_plugin_.WebviewShowOptions.md) |
| `options?` | [`WebviewPanelOptions`](../interfaces/codearts_plugin_.WebviewPanelOptions.md) & [`WebviewOptions`](../interfaces/codearts_plugin_.WebviewOptions.md) |

#### Returns

[`WebviewContainer`](../interfaces/codearts_plugin_.WebviewContainer.md)

#### Defined in

[index.d.ts:10059](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10059)

___

### createInputBox

▸ **createInputBox**(): [`InputBox`](../interfaces/codearts_plugin_.InputBox.md)

Creates a [InputBox](../interfaces/codearts_plugin_.InputBox.md) to let the user enter some text input.

Note that in many cases the more convenient [showInputBox](codearts_plugin_.window.md#showinputbox)
is easier to use. [createInputBox](codearts_plugin_.window.md#createinputbox) should be used
when [showInputBox](codearts_plugin_.window.md#showinputbox) does not offer the required flexibility.

#### Returns

[`InputBox`](../interfaces/codearts_plugin_.InputBox.md)

A new [InputBox](../interfaces/codearts_plugin_.InputBox.md).

#### Defined in

[index.d.ts:10017](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10017)

___

### createLightWebviewPanel

▸ **createLightWebviewPanel**(`viewType`, `title`, `showOptions`, `options?`): [`WebviewContainer`](../interfaces/codearts_plugin_.WebviewContainer.md)

Compared with `createWebviewPanel`, webview be created not only in editor area, but also can be resided in a specify panel area.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewType` | `string` | Identifies the type of the webview panel. |
| `title` | `string` | Title of the panel. |
| `showOptions` | [`WebviewShowOptions`](../interfaces/codearts_plugin_.WebviewShowOptions.md) | where webview panel will be reside. If preserveFocus is set, the new webview will not take focus. |
| `options?` | [`WebviewPanelOptions`](../interfaces/codearts_plugin_.WebviewPanelOptions.md) & [`WebviewOptions`](../interfaces/codearts_plugin_.WebviewOptions.md) | Settings for the new panel. |

#### Returns

[`WebviewContainer`](../interfaces/codearts_plugin_.WebviewContainer.md)

New webview panel.

#### Defined in

[index.d.ts:10053](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10053)

___

### createOutputChannel

▸ **createOutputChannel**(`name`, `languageId?`): [`OutputChannel`](../interfaces/codearts_plugin_.OutputChannel.md)

Creates a new [output channel](../interfaces/codearts_plugin_.OutputChannel.md) with the given name and language id
If language id is not provided, then **Log** is used as default language id.

You can access the visible or active output channel as a [text document](../interfaces/codearts_plugin_.TextDocument.md) from [visible editors](codearts_plugin_.window.md#visibletexteditors) or [active editor](codearts_plugin_.window.md#activetexteditor)
and use the language id to contribute language features like syntax coloring, code lens etc.,

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Human-readable string which will be used to represent the channel in the UI. |
| `languageId?` | `string` | The identifier of the language associated with the channel. |

#### Returns

[`OutputChannel`](../interfaces/codearts_plugin_.OutputChannel.md)

#### Defined in

[index.d.ts:10029](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10029)

___

### createQuickPick

▸ **createQuickPick**<`T`\>(): [`QuickPick`](../interfaces/codearts_plugin_.QuickPick.md)<`T`\>

Creates a [QuickPick](../interfaces/codearts_plugin_.QuickPick.md) to let the user pick an item from a list
of items of type T.

Note that in many cases the more convenient [showQuickPick](codearts_plugin_.window.md#showquickpick)
is easier to use. [createQuickPick](codearts_plugin_.window.md#createquickpick) should be used
when [showQuickPick](codearts_plugin_.window.md#showquickpick) does not offer the required flexibility.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`QuickPickItem`](../interfaces/codearts_plugin_.QuickPickItem.md) |

#### Returns

[`QuickPick`](../interfaces/codearts_plugin_.QuickPick.md)<`T`\>

A new [QuickPick](../interfaces/codearts_plugin_.QuickPick.md).

#### Defined in

[index.d.ts:10006](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10006)

___

### createStatusBarItem

▸ **createStatusBarItem**(`alignment?`, `priority?`): [`StatusBarItem`](../interfaces/codearts_plugin_.StatusBarItem.md)

Creates a status bar [item](../interfaces/codearts_plugin_.StatusBarItem.md).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `alignment?` | [`StatusBarAlignment`](../enums/codearts_plugin_.StatusBarAlignment.md) | The alignment of the item. |
| `priority?` | `number` | The priority of the item. Higher values mean the item should be shown more to the left. |

#### Returns

[`StatusBarItem`](../interfaces/codearts_plugin_.StatusBarItem.md)

A new status bar item.

#### Defined in

[index.d.ts:10133](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10133)

▸ **createStatusBarItem**(`id`, `alignment?`, `priority?`): [`StatusBarItem`](../interfaces/codearts_plugin_.StatusBarItem.md)

Creates a status bar [item](../interfaces/codearts_plugin_.StatusBarItem.md).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | The unique identifier of the item. |
| `alignment?` | [`StatusBarAlignment`](../enums/codearts_plugin_.StatusBarAlignment.md) | The alignment of the item. |
| `priority?` | `number` | The priority of the item. Higher values mean the item should be shown more to the left. |

#### Returns

[`StatusBarItem`](../interfaces/codearts_plugin_.StatusBarItem.md)

A new status bar item.

#### Defined in

[index.d.ts:10143](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10143)

___

### createTerminal

▸ **createTerminal**(`name?`, `shellPath?`, `shellArgs?`): [`Terminal`](../interfaces/codearts_plugin_.Terminal.md)

Creates a [Terminal](../interfaces/codearts_plugin_.Terminal.md) with a backing shell process. The cwd of the terminal will be the workspace
directory if it exists.

**`Throws`**

When running in an environment where a new process cannot be started.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name?` | `string` | Optional human-readable string which will be used to represent the terminal in the UI. |
| `shellPath?` | `string` | Optional path to a custom shell executable to be used in the terminal. |
| `shellArgs?` | `string` \| readonly `string`[] | Optional args for the custom shell executable. A string can be used on Windows only which allows specifying shell args in [command-line format](https://msdn.microsoft.com/en-au/08dfcab2-eb6e-49a4-80eb-87d4076c98c6). |

#### Returns

[`Terminal`](../interfaces/codearts_plugin_.Terminal.md)

A new Terminal.

#### Defined in

[index.d.ts:10157](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10157)

▸ **createTerminal**(`options`): [`Terminal`](../interfaces/codearts_plugin_.Terminal.md)

Creates a [Terminal](../interfaces/codearts_plugin_.Terminal.md) with a backing shell process.

**`Throws`**

When running in an environment where a new process cannot be started.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`TerminalOptions`](../interfaces/codearts_plugin_.TerminalOptions.md) | A TerminalOptions object describing the characteristics of the new terminal. |

#### Returns

[`Terminal`](../interfaces/codearts_plugin_.Terminal.md)

A new Terminal.

#### Defined in

[index.d.ts:10166](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10166)

▸ **createTerminal**(`options`): [`Terminal`](../interfaces/codearts_plugin_.Terminal.md)

Creates a [Terminal](../interfaces/codearts_plugin_.Terminal.md) where an extension controls its input and output.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`ExtensionTerminalOptions`](../interfaces/codearts_plugin_.ExtensionTerminalOptions.md) | An [ExtensionTerminalOptions](../interfaces/codearts_plugin_.ExtensionTerminalOptions.md) object describing the characteristics of the new terminal. |

#### Returns

[`Terminal`](../interfaces/codearts_plugin_.Terminal.md)

A new Terminal.

#### Defined in

[index.d.ts:10175](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10175)

___

### createTextEditorDecorationType

▸ **createTextEditorDecorationType**(`options`): [`TextEditorDecorationType`](../interfaces/codearts_plugin_.TextEditorDecorationType.md)

Create a TextEditorDecorationType that can be used to add decorations to text editors.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`DecorationRenderOptions`](../interfaces/codearts_plugin_.DecorationRenderOptions.md) | Rendering options for the decoration type. |

#### Returns

[`TextEditorDecorationType`](../interfaces/codearts_plugin_.TextEditorDecorationType.md)

A new decoration type instance.

#### Defined in

[index.d.ts:9778](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9778)

___

### createTreeView

▸ **createTreeView**<`T`\>(`viewId`, `options`): [`TreeView`](../interfaces/codearts_plugin_.TreeView.md)<`T`\>

Create a [TreeView](../interfaces/codearts_plugin_.TreeView.md) for the view contributed using the extension point `views`.

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewId` | `string` | Id of the view contributed using the extension point `views`. |
| `options` | [`TreeViewOptions`](../interfaces/codearts_plugin_.TreeViewOptions.md)<`T`\> | Options for creating the [TreeView](../interfaces/codearts_plugin_.TreeView.md) |

#### Returns

[`TreeView`](../interfaces/codearts_plugin_.TreeView.md)<`T`\>

a [TreeView](../interfaces/codearts_plugin_.TreeView.md).

#### Defined in

[index.d.ts:10202](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10202)

___

### createWebviewPanel

▸ **createWebviewPanel**(`viewType`, `title`, `showOptions`, `options?`): [`WebviewPanel`](../interfaces/codearts_plugin_.WebviewPanel.md)

Create and show a new webview panel.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewType` | `string` | Identifies the type of the webview panel. |
| `title` | `string` | Title of the panel. |
| `showOptions` | [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md) \| { `preserveFocus?`: `boolean` ; `viewColumn`: [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md)  } | Where to show the webview in the editor. If preserveFocus is set, the new webview will not take focus. |
| `options?` | [`WebviewPanelOptions`](../interfaces/codearts_plugin_.WebviewPanelOptions.md) & [`WebviewOptions`](../interfaces/codearts_plugin_.WebviewOptions.md) | Settings for the new panel. |

#### Returns

[`WebviewPanel`](../interfaces/codearts_plugin_.WebviewPanel.md)

New webview panel.

#### Defined in

[index.d.ts:10041](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10041)

___

### createWebviewViewDialog

▸ **createWebviewViewDialog**(`provider`, `dialogOptions`): [`WebviewViewDialog`](../interfaces/codearts_plugin_.WebviewViewDialog.md)

Create and open a dialog with an webview view.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `provider` | [`WebviewViewProvider`](../interfaces/codearts_plugin_.WebviewViewProvider.md) | Provider for the webview views. |
| `dialogOptions` | [`DialogOptions`](../interfaces/codearts_plugin_.DialogOptions.md) | - |

#### Returns

[`WebviewViewDialog`](../interfaces/codearts_plugin_.WebviewViewDialog.md)

Disposable that unregister the provider.

#### Defined in

[index.d.ts:10290](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10290)

___

### getTerminalById

▸ **getTerminalById**(`id`): [`Terminal`](../interfaces/codearts_plugin_.Terminal.md) \| `undefined`

Get terminal by it's unique id.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | The unique id for terminal |

#### Returns

[`Terminal`](../interfaces/codearts_plugin_.Terminal.md) \| `undefined`

Terminal or undefined.

#### Defined in

[index.d.ts:10183](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10183)

___

### onDidChangeActiveColorTheme

▸ **onDidChangeActiveColorTheme**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`ColorTheme`](../interfaces/codearts_plugin_.ColorTheme.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidChangeActiveNotebookEditor

▸ **onDidChangeActiveNotebookEditor**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: `undefined` \| [`NotebookEditor`](../interfaces/codearts_plugin_.NotebookEditor.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidChangeActiveTerminal

▸ **onDidChangeActiveTerminal**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: `undefined` \| [`Terminal`](../interfaces/codearts_plugin_.Terminal.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidChangeActiveTextEditor

▸ **onDidChangeActiveTextEditor**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: `undefined` \| [`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidChangeNotebookEditorSelection

▸ **onDidChangeNotebookEditorSelection**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`NotebookEditorSelectionChangeEvent`](../interfaces/codearts_plugin_.NotebookEditorSelectionChangeEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidChangeNotebookEditorVisibleRanges

▸ **onDidChangeNotebookEditorVisibleRanges**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`NotebookEditorVisibleRangesChangeEvent`](../interfaces/codearts_plugin_.NotebookEditorVisibleRangesChangeEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidChangeTerminalColor

▸ **onDidChangeTerminalColor**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TerminalColorChangeEvent`](../interfaces/codearts_plugin_.TerminalColorChangeEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidChangeTerminalState

▸ **onDidChangeTerminalState**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`Terminal`](../interfaces/codearts_plugin_.Terminal.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidChangeTextEditorOptions

▸ **onDidChangeTextEditorOptions**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TextEditorOptionsChangeEvent`](../interfaces/codearts_plugin_.TextEditorOptionsChangeEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidChangeTextEditorSelection

▸ **onDidChangeTextEditorSelection**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TextEditorSelectionChangeEvent`](../interfaces/codearts_plugin_.TextEditorSelectionChangeEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidChangeTextEditorViewColumn

▸ **onDidChangeTextEditorViewColumn**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TextEditorViewColumnChangeEvent`](../interfaces/codearts_plugin_.TextEditorViewColumnChangeEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidChangeTextEditorVisibleRanges

▸ **onDidChangeTextEditorVisibleRanges**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TextEditorVisibleRangesChangeEvent`](../interfaces/codearts_plugin_.TextEditorVisibleRangesChangeEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidChangeVisibleNotebookEditors

▸ **onDidChangeVisibleNotebookEditors**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: readonly [`NotebookEditor`](../interfaces/codearts_plugin_.NotebookEditor.md)[]) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidChangeVisibleTextEditors

▸ **onDidChangeVisibleTextEditors**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: readonly [`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)[]) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidChangeWindowState

▸ **onDidChangeWindowState**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`WindowState`](../interfaces/codearts_plugin_.WindowState.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidCloseTerminal

▸ **onDidCloseTerminal**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`Terminal`](../interfaces/codearts_plugin_.Terminal.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidOpenTerminal

▸ **onDidOpenTerminal**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`Terminal`](../interfaces/codearts_plugin_.Terminal.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### onDidRenameTerminal

▸ **onDidRenameTerminal**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`Terminal`](../interfaces/codearts_plugin_.Terminal.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L1603)

___

### registerComponentsInEditorGutter

▸ **registerComponentsInEditorGutter**(`filePath`, `components`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register components to editor gutter in batches

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `filePath` | `string` | File path of document where components are registered. (Notes:   The value of this arg should be the same with 'editor.document.uri.fsPath'.) |
| `components` | [`Component`](../interfaces/codearts_plugin_.ui.Component.md)[] | Components to be registered in batches. (Notes:   1. The array stores components in different positions of the filePath.   2. If this arg is an empty array, the components of the filePath will be unregistered.   3. If this arg is not an empty array, all components of the filePath that have been registered last time will be unregistered and replaced by components that are going to be registered this time.) |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

Disposable which unregisters this command on disposal.

#### Defined in

[index.d.ts:9584](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9584)

___

### registerCustomEditorProvider

▸ **registerCustomEditorProvider**(`viewType`, `provider`, `options?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a provider for custom editors for the `viewType` contributed by the `customEditors` extension point.

When a custom editor is opened, an `onCustomEditor:viewType` activation event is fired. Your extension
must register a [`CustomTextEditorProvider`](../interfaces/codearts_plugin_.CustomTextEditorProvider.md), [`CustomReadonlyEditorProvider`](../interfaces/codearts_plugin_.CustomReadonlyEditorProvider.md),
[`CustomEditorProvider`](../interfaces/codearts_plugin_.CustomEditorProvider.md)for `viewType` as part of activation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewType` | `string` | Unique identifier for the custom editor provider. This should match the `viewType` from the   `customEditors` contribution point. |
| `provider` | [`CustomTextEditorProvider`](../interfaces/codearts_plugin_.CustomTextEditorProvider.md) \| [`CustomReadonlyEditorProvider`](../interfaces/codearts_plugin_.CustomReadonlyEditorProvider.md)<[`CustomDocument`](../interfaces/codearts_plugin_.CustomDocument.md)\> \| [`CustomEditorProvider`](../interfaces/codearts_plugin_.CustomEditorProvider.md)<[`CustomDocument`](../interfaces/codearts_plugin_.CustomDocument.md)\> | Provider that resolves custom editors. |
| `options?` | `Object` | Options for the provider. |
| `options.supportsMultipleEditorsPerDocument?` | `boolean` | Only applies to `CustomReadonlyEditorProvider \| CustomEditorProvider`.  Indicates that the provider allows multiple editor instances to be open at the same time for the same resource.  By default, the editor only allows one editor instance to be open at a time for each resource. If the user tries to open a second editor instance for the resource, the first one is instead moved to where the second one was to be opened.  When `supportsMultipleEditorsPerDocument` is enabled, users can split and create copies of the custom editor. In this case, the custom editor must make sure it can properly synchronize the states of all editor instances for a resource so that they are consistent. |
| `options.webviewOptions?` | [`WebviewPanelOptions`](../interfaces/codearts_plugin_.WebviewPanelOptions.md) | Content settings for the webview panels created for this custom editor. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

Disposable that unregisters the provider.

#### Defined in

[index.d.ts:10306](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10306)

___

### registerFileDecorationProvider

▸ **registerFileDecorationProvider**(`provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a file decoration provider.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `provider` | [`FileDecorationProvider`](../interfaces/codearts_plugin_.FileDecorationProvider.md) | A [FileDecorationProvider](../interfaces/codearts_plugin_.FileDecorationProvider.md). |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters the provider.

#### Defined in

[index.d.ts:10348](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10348)

___

### registerMainMenu

▸ **registerMainMenu**(`item`, `side?`): `void`

Register a top level menu on titlepart area.

**`Deprecated`**

Recommend to use registerMenu.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`MenuItem`](../interfaces/codearts_plugin_.MenuItem.md) \| [`SubmenuItem`](../interfaces/codearts_plugin_.SubmenuItem.md) | The actual menu or submenu. |
| `side?` | [`MenuSide`](../enums/codearts_plugin_.MenuSide.md) | The side of titlepart. |

#### Returns

`void`

#### Defined in

[index.d.ts:10367](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10367)

___

### registerMenu

▸ **registerMenu**(`id`, `item`): `void`

Register menu or submenu using menu id.

*Note* that if the menuId is not registered before, it will be registered automatically.
Make sure a menuId is already registered before using it.

**Example:** Register a submenu 'Hello' in 'File' menu, and menu 'Command Palette' under 'Hello'.
```typescript
// Register a menu 'Command Palette' under submenu 'Hello', the menuId 'HelloMenuId' will be registered automatically
vscode.window.registerMenu('HelloMenuId', { command: { id: 'workbench.action.showCommands', title: 'Command Palette'} });

// Register the submenu 'Hello' in 'File' menu for which the menuId is 'MenubarFileMenu'
vscode.window.registerMenu('MenubarFileMenu', { submenu: 'HelloMenuId', title: 'Hello' });
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | Menu id. |
| `item` | [`MenuItem`](../interfaces/codearts_plugin_.MenuItem.md) \| [`SubmenuItem`](../interfaces/codearts_plugin_.SubmenuItem.md) | The actual menu or submenu. |

#### Returns

`void`

#### Defined in

[index.d.ts:10387](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10387)

___

### registerMenuId

▸ **registerMenuId**(`id`): `void`

Register a custom menu id. Must call it before registerMenu

**`Deprecated`**

Recommend to use registerMenu. Now registerMenu will register id automatically.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | custom menu id. |

#### Returns

`void`

#### Defined in

[index.d.ts:10394](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10394)

___

### registerProjectWizardProvider

▸ **registerProjectWizardProvider**(`id`, `label`, `provider`, `options?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a provider for project wizard with webview view.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | Unique id of the project wizard. |
| `label` | `string` | Label of the project wizard, like 'java', 'c++'. |
| `provider` | [`WebviewViewProvider`](../interfaces/codearts_plugin_.WebviewViewProvider.md) | Webview view provider. |
| `options?` | [`ProjectWizardOptions`](../interfaces/codearts_plugin_.ProjectWizardOptions.md) | [ProjectWizardOptions](../interfaces/codearts_plugin_.ProjectWizardOptions.md) Options of the project wizard. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

Disposable that unregisters the provider.

#### Defined in

[index.d.ts:10283](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10283)

___

### registerTerminalLinkProvider

▸ **registerTerminalLinkProvider**(`provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register provider that enables the detection and handling of links within the terminal.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `provider` | [`TerminalLinkProvider`](../interfaces/codearts_plugin_.TerminalLinkProvider.md)<[`TerminalLink`](../classes/codearts_plugin_.TerminalLink.md)\> | The provider that provides the terminal links. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

Disposable that unregisters the provider.

#### Defined in

[index.d.ts:10334](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10334)

___

### registerTerminalProfileProvider

▸ **registerTerminalProfileProvider**(`id`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Registers a provider for a contributed terminal profile.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | The ID of the contributed terminal profile. |
| `provider` | [`TerminalProfileProvider`](../interfaces/codearts_plugin_.TerminalProfileProvider.md) | The terminal profile provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:10341](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10341)

___

### registerTreeDataProvider

▸ **registerTreeDataProvider**<`T`\>(`viewId`, `treeDataProvider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a [TreeDataProvider](../interfaces/codearts_plugin_.TreeDataProvider.md) for the view contributed using the extension point `views`.
This will allow you to contribute data to the [TreeView](../interfaces/codearts_plugin_.TreeView.md) and update if the data changes.

**Note:** To get access to the [TreeView](../interfaces/codearts_plugin_.TreeView.md) and perform operations on it, use [createTreeView](codearts_plugin_.window.md#createtreeview).

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewId` | `string` | Id of the view contributed using the extension point `views`. |
| `treeDataProvider` | [`TreeDataProvider`](../interfaces/codearts_plugin_.TreeDataProvider.md)<`T`\> | A [TreeDataProvider](../interfaces/codearts_plugin_.TreeDataProvider.md) that provides tree data for the view |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:10194](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10194)

___

### registerUriHandler

▸ **registerUriHandler**(`handler`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Registers a [uri handler](../interfaces/codearts_plugin_.UriHandler.md) capable of handling system-wide [uris](../classes/codearts_plugin_.Uri.md).
In case there are multiple windows open, the topmost window will handle the uri.
A uri handler is scoped to the extension it is contributed from; it will only
be able to handle uris which are directed to the extension itself. A uri must respect
the following rules:

- The uri-scheme must be `vscode.env.uriScheme`;
- The uri-authority must be the extension id (e.g. `my.extension`);
- The uri-path, -query and -fragment parts are arbitrary.

For example, if the `my.extension` extension registers a uri handler, it will only
be allowed to handle uris with the prefix `product-name://my.extension`.

An extension can only register a single uri handler in its entire activation lifetime.

* *Note:* There is an activation event `onUri` that fires when a uri directed for
the current extension is about to be handled.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `handler` | [`UriHandler`](../interfaces/codearts_plugin_.UriHandler.md) | The uri handler to register for this extension. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:10225](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10225)

___

### registerViewContainerSubTitle

▸ **registerViewContainerSubTitle**(`viewContainerId`, `title`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register the subtitle of a non-built-in container. If the container does not have a subtitle, add it. If the container already has a subtitle, update it.

**Example:** Register a subtitle 'subTitle' in 'package-explorer' extension.
```typescript
const viewContainerId = 'package-explorer';
vscode.window.registerViewContainerSubTitle(viewContainerId, 'subTitle' });
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewContainerId` | `string` | ID of the ViewContainer. |
| `title` | `string` | Subtitle of the container to be registered. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9570](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9570)

___

### registerViewTitleActions

▸ **registerViewTitleActions**(`location`, `actionViewItems`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register actions to specific view using location which support view, viewContainer or editor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `location` | [`ViewLocation`](_codearts_plugin_.md#viewlocation) | Location where Actions are registered. |
| `actionViewItems` | [`ActionViewItem`](../interfaces/codearts_plugin_.ui.ActionViewItem-1.md) \| [`ActionViewItem`](../interfaces/codearts_plugin_.ui.ActionViewItem-1.md)[] | Components to be registered. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

Disposable which unregisters this command on disposal.

#### Defined in

[index.d.ts:9556](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9556)

___

### registerWebviewPanelSerializer

▸ **registerWebviewPanelSerializer**(`viewType`, `serializer`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Registers a webview panel serializer.

Extensions that support reviving should have an `"onWebviewPanel:viewType"` activation event and
make sure that `registerWebviewPanelSerializer` is called during activation.

Only a single serializer may be registered at a time for a given `viewType`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewType` | `string` | Type of the webview panel that can be serialized. |
| `serializer` | [`WebviewPanelSerializer`](../interfaces/codearts_plugin_.WebviewPanelSerializer.md)<`unknown`\> | Webview serializer. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:10238](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10238)

___

### registerWebviewViewProvider

▸ **registerWebviewViewProvider**(`viewId`, `provider`, `options?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a new provider for webview views.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewId` | `string` | Unique id of the view. This should match the `id` from the   `views` contribution in the package.json. |
| `provider` | [`WebviewViewProvider`](../interfaces/codearts_plugin_.WebviewViewProvider.md) | Provider for the webview views. |
| `options?` | `Object` | - |
| `options.webviewOptions?` | `Object` | Content settings for the webview created for this view. |
| `options.webviewOptions.retainContextWhenHidden?` | `boolean` | Controls if the webview element itself (iframe) is kept around even when the view is no longer visible.  Normally the webview's html context is created when the view becomes visible and destroyed when it is hidden. Extensions that have complex state or UI can set the `retainContextWhenHidden` to make the editor keep the webview context around, even when the webview moves to a background tab. When a webview using `retainContextWhenHidden` becomes hidden, its scripts and other dynamic content are suspended. When the view becomes visible again, the context is automatically restored in the exact same state it was in originally. You cannot send messages to a hidden webview, even with `retainContextWhenHidden` enabled.  `retainContextWhenHidden` has a high memory overhead and should only be used if your view's context cannot be quickly saved and restored. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

Disposable that unregisters the provider.

#### Defined in

[index.d.ts:10249](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10249)

___

### setStatusBarMessage

▸ **setStatusBarMessage**(`text`, `hideAfterTimeout`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Set a message to the status bar. This is a short hand for the more powerful
status bar [items](codearts_plugin_.window.md#createstatusbaritem).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` | The message to show, supports icon substitution as in status bar [items](../interfaces/codearts_plugin_.StatusBarItem.md#text). |
| `hideAfterTimeout` | `number` | Timeout in milliseconds after which the message will be disposed. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which hides the status bar message.

#### Defined in

[index.d.ts:10069](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10069)

▸ **setStatusBarMessage**(`text`, `hideWhenDone`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Set a message to the status bar. This is a short hand for the more powerful
status bar [items](codearts_plugin_.window.md#createstatusbaritem).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` | The message to show, supports icon substitution as in status bar [items](../interfaces/codearts_plugin_.StatusBarItem.md#text). |
| `hideWhenDone` | [`Thenable`](../interfaces/Thenable.md)<`any`\> | Thenable on which completion (resolve or reject) the message will be disposed. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which hides the status bar message.

#### Defined in

[index.d.ts:10079](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10079)

▸ **setStatusBarMessage**(`text`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Set a message to the status bar. This is a short hand for the more powerful
status bar [items](codearts_plugin_.window.md#createstatusbaritem).

*Note* that status bar messages stack and that they must be disposed when no
longer used.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` | The message to show, supports icon substitution as in status bar [items](../interfaces/codearts_plugin_.StatusBarItem.md#text). |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which hides the status bar message.

#### Defined in

[index.d.ts:10091](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10091)

___

### showCodeTip

▸ **showCodeTip**(`message`, `position`, `options?`): `void`

Show simple code message tip in the active editor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` |  |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) | Editor position. If the input line number or character number exceeds the maximum, the tip will display at the end of the code area. If the number is less than 0, it will be set to 0. |
| `options?` | [`CodeTipOptions`](../interfaces/codearts_plugin_.CodeTipOptions.md) | [CodeTipOptions](../interfaces/codearts_plugin_.CodeTipOptions.md) to configure the behavior of showing the code tip |

#### Returns

`void`

#### Defined in

[index.d.ts:10417](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10417)

___

### showErrorMessage

▸ **showErrorMessage**<`T`\>(`message`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

Show an error message.

**`See`**

[showInformationMessage](codearts_plugin_.window.md#showinformationmessage)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `string` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | The message to show. |
| `...items` | `T`[] | A set of items that will be rendered as actions in the message. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

A thenable that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:9879](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9879)

▸ **showErrorMessage**<`T`\>(`message`, `options`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

Show an error message.

**`See`**

[showInformationMessage](codearts_plugin_.window.md#showinformationmessage)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `string` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | The message to show. |
| `options` | [`MessageOptions`](../interfaces/codearts_plugin_.MessageOptions.md) | Configures the behaviour of the message. |
| `...items` | `T`[] | A set of items that will be rendered as actions in the message. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

A thenable that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:9891](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9891)

▸ **showErrorMessage**<`T`\>(`message`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

Show an error message.

**`See`**

[showInformationMessage](codearts_plugin_.window.md#showinformationmessage)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`MessageItem`](../interfaces/codearts_plugin_.MessageItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | The message to show. |
| `...items` | `T`[] | A set of items that will be rendered as actions in the message. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

A thenable that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:9902](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9902)

▸ **showErrorMessage**<`T`\>(`message`, `options`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

Show an error message.

**`See`**

[showInformationMessage](codearts_plugin_.window.md#showinformationmessage)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`MessageItem`](../interfaces/codearts_plugin_.MessageItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | The message to show. |
| `options` | [`MessageOptions`](../interfaces/codearts_plugin_.MessageOptions.md) | Configures the behaviour of the message. |
| `...items` | `T`[] | A set of items that will be rendered as actions in the message. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

A thenable that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:9914](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9914)

___

### showInformationMessage

▸ **showInformationMessage**<`T`\>(`message`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

Show an information message to users. Optionally provide an array of items which will be presented as
clickable buttons.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `string` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | The message to show. |
| `...items` | `T`[] | A set of items that will be rendered as actions in the message. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

A thenable that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:9788](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9788)

▸ **showInformationMessage**<`T`\>(`message`, `options`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

Show an information message to users. Optionally provide an array of items which will be presented as
clickable buttons.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `string` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | The message to show. |
| `options` | [`MessageOptions`](../interfaces/codearts_plugin_.MessageOptions.md) | Configures the behaviour of the message. |
| `...items` | `T`[] | A set of items that will be rendered as actions in the message. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

A thenable that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:9799](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9799)

▸ **showInformationMessage**<`T`\>(`message`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

Show an information message.

**`See`**

[showInformationMessage](codearts_plugin_.window.md#showinformationmessage)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`MessageItem`](../interfaces/codearts_plugin_.MessageItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | The message to show. |
| `...items` | `T`[] | A set of items that will be rendered as actions in the message. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

A thenable that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:9810](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9810)

▸ **showInformationMessage**<`T`\>(`message`, `options`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

Show an information message.

**`See`**

[showInformationMessage](codearts_plugin_.window.md#showinformationmessage)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`MessageItem`](../interfaces/codearts_plugin_.MessageItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | The message to show. |
| `options` | [`MessageOptions`](../interfaces/codearts_plugin_.MessageOptions.md) | Configures the behaviour of the message. |
| `...items` | `T`[] | A set of items that will be rendered as actions in the message. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

A thenable that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:9822](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9822)

___

### showInputBox

▸ **showInputBox**(`options?`, `token?`): [`Thenable`](../interfaces/Thenable.md)<`string` \| `undefined`\>

Opens an input box to ask the user for input.

The returned value will be `undefined` if the input box was canceled (e.g. pressing ESC). Otherwise the
returned value will be the string typed by the user or an empty string if the user did not type
anything but dismissed the input box with OK.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | [`InputBoxOptions`](../interfaces/codearts_plugin_.InputBoxOptions.md) | Configures the behavior of the input box. |
| `token?` | [`CancellationToken`](../interfaces/codearts_plugin_.CancellationToken.md) | A token that can be used to signal cancellation. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`string` \| `undefined`\>

A promise that resolves to a string the user provided or to `undefined` in case of dismissal.

#### Defined in

[index.d.ts:9994](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9994)

___

### showNotebookDocument

▸ **showNotebookDocument**(`document`, `options?`): [`Thenable`](../interfaces/Thenable.md)<[`NotebookEditor`](../interfaces/codearts_plugin_.NotebookEditor.md)\>

Show the given [NotebookDocument](../interfaces/codearts_plugin_.NotebookDocument.md) in a [notebook editor](../interfaces/codearts_plugin_.NotebookEditor.md).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md) | A text document to be shown. |
| `options?` | [`NotebookDocumentShowOptions`](../interfaces/codearts_plugin_.NotebookDocumentShowOptions.md) | [Editor options](../interfaces/codearts_plugin_.NotebookDocumentShowOptions.md) to configure the behavior of showing the [notebook editor](../interfaces/codearts_plugin_.NotebookEditor.md). |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`NotebookEditor`](../interfaces/codearts_plugin_.NotebookEditor.md)\>

A promise that resolves to an [notebook editor](../interfaces/codearts_plugin_.NotebookEditor.md).

#### Defined in

[index.d.ts:9770](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9770)

___

### showOpenDialog

▸ **showOpenDialog**(`options?`): [`Thenable`](../interfaces/Thenable.md)<[`Uri`](../classes/codearts_plugin_.Uri.md)[] \| `undefined`\>

Shows a file open dialog to the user which allows to select a file
for opening-purposes.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | [`OpenDialogOptions`](../interfaces/codearts_plugin_.OpenDialogOptions.md) | Options that control the dialog. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`Uri`](../classes/codearts_plugin_.Uri.md)[] \| `undefined`\>

A promise that resolves to the selected resources or `undefined`.

#### Defined in

[index.d.ts:9972](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9972)

___

### showQuickPick

▸ **showQuickPick**(`items`, `options`, `token?`): [`Thenable`](../interfaces/Thenable.md)<`string`[] \| `undefined`\>

Shows a selection list allowing multiple selections.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `items` | readonly `string`[] \| [`Thenable`](../interfaces/Thenable.md)<readonly `string`[]\> | An array of strings, or a promise that resolves to an array of strings. |
| `options` | [`QuickPickOptions`](../interfaces/codearts_plugin_.QuickPickOptions.md) & { `canPickMany`: ``true``  } | Configures the behavior of the selection list. |
| `token?` | [`CancellationToken`](../interfaces/codearts_plugin_.CancellationToken.md) | A token that can be used to signal cancellation. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`string`[] \| `undefined`\>

A promise that resolves to the selected items or `undefined`.

#### Defined in

[index.d.ts:9924](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9924)

▸ **showQuickPick**(`items`, `options?`, `token?`): [`Thenable`](../interfaces/Thenable.md)<`string` \| `undefined`\>

Shows a selection list.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `items` | readonly `string`[] \| [`Thenable`](../interfaces/Thenable.md)<readonly `string`[]\> | An array of strings, or a promise that resolves to an array of strings. |
| `options?` | [`QuickPickOptions`](../interfaces/codearts_plugin_.QuickPickOptions.md) | Configures the behavior of the selection list. |
| `token?` | [`CancellationToken`](../interfaces/codearts_plugin_.CancellationToken.md) | A token that can be used to signal cancellation. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`string` \| `undefined`\>

A promise that resolves to the selection or `undefined`.

#### Defined in

[index.d.ts:9934](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9934)

▸ **showQuickPick**<`T`\>(`items`, `options`, `token?`): [`Thenable`](../interfaces/Thenable.md)<`T`[] \| `undefined`\>

Shows a selection list allowing multiple selections.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`QuickPickItem`](../interfaces/codearts_plugin_.QuickPickItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `items` | readonly `T`[] \| [`Thenable`](../interfaces/Thenable.md)<readonly `T`[]\> | An array of items, or a promise that resolves to an array of items. |
| `options` | [`QuickPickOptions`](../interfaces/codearts_plugin_.QuickPickOptions.md) & { `canPickMany`: ``true``  } | Configures the behavior of the selection list. |
| `token?` | [`CancellationToken`](../interfaces/codearts_plugin_.CancellationToken.md) | A token that can be used to signal cancellation. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T`[] \| `undefined`\>

A promise that resolves to the selected items or `undefined`.

#### Defined in

[index.d.ts:9944](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9944)

▸ **showQuickPick**<`T`\>(`items`, `options?`, `token?`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

Shows a selection list.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`QuickPickItem`](../interfaces/codearts_plugin_.QuickPickItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `items` | readonly `T`[] \| [`Thenable`](../interfaces/Thenable.md)<readonly `T`[]\> | An array of items, or a promise that resolves to an array of items. |
| `options?` | [`QuickPickOptions`](../interfaces/codearts_plugin_.QuickPickOptions.md) | Configures the behavior of the selection list. |
| `token?` | [`CancellationToken`](../interfaces/codearts_plugin_.CancellationToken.md) | A token that can be used to signal cancellation. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

A promise that resolves to the selected item or `undefined`.

#### Defined in

[index.d.ts:9954](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9954)

___

### showSaveDialog

▸ **showSaveDialog**(`options?`): [`Thenable`](../interfaces/Thenable.md)<[`Uri`](../classes/codearts_plugin_.Uri.md) \| `undefined`\>

Shows a file save dialog to the user which allows to select a file
for saving-purposes.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | [`SaveDialogOptions`](../interfaces/codearts_plugin_.SaveDialogOptions.md) | Options that control the dialog. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`Uri`](../classes/codearts_plugin_.Uri.md) \| `undefined`\>

A promise that resolves to the selected resource or `undefined`.

#### Defined in

[index.d.ts:9981](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9981)

___

### showTextDocument

▸ **showTextDocument**(`document`, `column?`, `preserveFocus?`): [`Thenable`](../interfaces/Thenable.md)<[`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)\>

Show the given document in a text editor. A [column](../enums/codearts_plugin_.ViewColumn.md) can be provided
to control where the editor is being shown. Might change the [active editor](codearts_plugin_.window.md#activetexteditor).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md) | A text document to be shown. |
| `column?` | [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md) | A view column in which the [editor](../interfaces/codearts_plugin_.TextEditor.md) should be shown. The default is the [active](../enums/codearts_plugin_.ViewColumn.md#active), other values are adjusted to be `Min(column, columnCount + 1)`, the [active](../enums/codearts_plugin_.ViewColumn.md#active)-column is not adjusted. Use [`Beside`](../enums/codearts_plugin_.ViewColumn.md#beside) to open the editor to the side of the currently active one. |
| `preserveFocus?` | `boolean` | When `true` the editor will not take focus. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)\>

A promise that resolves to an [editor](../interfaces/codearts_plugin_.TextEditor.md).

#### Defined in

[index.d.ts:9739](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9739)

▸ **showTextDocument**(`document`, `options?`): [`Thenable`](../interfaces/Thenable.md)<[`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)\>

Show the given document in a text editor. [Options](../interfaces/codearts_plugin_.TextDocumentShowOptions.md) can be provided
to control options of the editor is being shown. Might change the [active editor](codearts_plugin_.window.md#activetexteditor).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md) | A text document to be shown. |
| `options?` | [`TextDocumentShowOptions`](../interfaces/codearts_plugin_.TextDocumentShowOptions.md) | [Editor options](../interfaces/codearts_plugin_.TextDocumentShowOptions.md) to configure the behavior of showing the [editor](../interfaces/codearts_plugin_.TextEditor.md). |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)\>

A promise that resolves to an [editor](../interfaces/codearts_plugin_.TextEditor.md).

#### Defined in

[index.d.ts:9749](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9749)

▸ **showTextDocument**(`uri`, `options?`): [`Thenable`](../interfaces/Thenable.md)<[`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)\>

A short-hand for `openTextDocument(uri).then(document => showTextDocument(document, options))`.

**`See`**

[openTextDocument](codearts_plugin_.workspace.md#opentextdocument)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | A resource identifier. |
| `options?` | [`TextDocumentShowOptions`](../interfaces/codearts_plugin_.TextDocumentShowOptions.md) | [Editor options](../interfaces/codearts_plugin_.TextDocumentShowOptions.md) to configure the behavior of showing the [editor](../interfaces/codearts_plugin_.TextEditor.md). |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md)\>

A promise that resolves to an [editor](../interfaces/codearts_plugin_.TextEditor.md).

#### Defined in

[index.d.ts:9760](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9760)

___

### showWarningMessage

▸ **showWarningMessage**<`T`\>(`message`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

Show a warning message.

**`See`**

[showInformationMessage](codearts_plugin_.window.md#showinformationmessage)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `string` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | The message to show. |
| `...items` | `T`[] | A set of items that will be rendered as actions in the message. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

A thenable that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:9833](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9833)

▸ **showWarningMessage**<`T`\>(`message`, `options`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

Show a warning message.

**`See`**

[showInformationMessage](codearts_plugin_.window.md#showinformationmessage)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `string` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | The message to show. |
| `options` | [`MessageOptions`](../interfaces/codearts_plugin_.MessageOptions.md) | Configures the behaviour of the message. |
| `...items` | `T`[] | A set of items that will be rendered as actions in the message. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

A thenable that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:9845](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9845)

▸ **showWarningMessage**<`T`\>(`message`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

Show a warning message.

**`See`**

[showInformationMessage](codearts_plugin_.window.md#showinformationmessage)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`MessageItem`](../interfaces/codearts_plugin_.MessageItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | The message to show. |
| `...items` | `T`[] | A set of items that will be rendered as actions in the message. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

A thenable that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:9856](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9856)

▸ **showWarningMessage**<`T`\>(`message`, `options`, ...`items`): [`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

Show a warning message.

**`See`**

[showInformationMessage](codearts_plugin_.window.md#showinformationmessage)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`MessageItem`](../interfaces/codearts_plugin_.MessageItem.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | The message to show. |
| `options` | [`MessageOptions`](../interfaces/codearts_plugin_.MessageOptions.md) | Configures the behaviour of the message. |
| `...items` | `T`[] | A set of items that will be rendered as actions in the message. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T` \| `undefined`\>

A thenable that resolves to the selected item or `undefined` when being dismissed.

#### Defined in

[index.d.ts:9868](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9868)

___

### showWorkspaceFolderPick

▸ **showWorkspaceFolderPick**(`options?`): [`Thenable`](../interfaces/Thenable.md)<[`WorkspaceFolder`](../interfaces/codearts_plugin_.WorkspaceFolder.md) \| `undefined`\>

Shows a selection list of [workspace folders](codearts_plugin_.workspace.md#workspacefolders) to pick from.
Returns `undefined` if no folder is open.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | [`WorkspaceFolderPickOptions`](../interfaces/codearts_plugin_.WorkspaceFolderPickOptions.md) | Configures the behavior of the workspace folder list. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`WorkspaceFolder`](../interfaces/codearts_plugin_.WorkspaceFolder.md) \| `undefined`\>

A promise that resolves to the workspace folder or `undefined`.

#### Defined in

[index.d.ts:9963](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L9963)

___

### unregisterMainMenu

▸ **unregisterMainMenu**(`side`): `void`

Unregister menu on left or right side of titlepart.

**`Deprecated`**

Recommend to use unregisterMenu.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `side` | [`MenuSide`](../enums/codearts_plugin_.MenuSide.md) | The side of titlepart. |

#### Returns

`void`

#### Defined in

[index.d.ts:10401](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10401)

___

### unregisterMenu

▸ **unregisterMenu**(`id`): `void`

Unregister a menu. Extensions can not remove submenus registered by core and can only remove menus registered
by extensions.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | Custom submenu id. |

#### Returns

`void`

#### Defined in

[index.d.ts:10408](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10408)

___

### withProgress

▸ **withProgress**<`R`\>(`options`, `task`): [`Thenable`](../interfaces/Thenable.md)<`R`\>

Show progress in the editor. Progress is shown while running the given callback
and while the promise it returned isn't resolved nor rejected. The location at which
progress should show (and other details) is defined via the passed [`ProgressOptions`](../interfaces/codearts_plugin_.ProgressOptions.md).

#### Type parameters

| Name |
| :------ |
| `R` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`ProgressOptions`](../interfaces/codearts_plugin_.ProgressOptions.md) | - |
| `task` | (`progress`: [`Progress`](../interfaces/codearts_plugin_.Progress.md)<{ `increment?`: `number` ; `message?`: `string`  }\>, `token`: [`CancellationToken`](../interfaces/codearts_plugin_.CancellationToken.md)) => [`Thenable`](../interfaces/Thenable.md)<`R`\> | A callback returning a promise. Progress state can be reported with the provided [Progress](../interfaces/codearts_plugin_.Progress.md)-object.  To report discrete progress, use `increment` to indicate how much work has been completed. Each call with a `increment` value will be summed up and reflected as overall progress until 100% is reached (a value of e.g. `10` accounts for `10%` of work done). Note that currently only `ProgressLocation.Notification` is capable of showing discrete progress.  To monitor if the operation has been cancelled by the user, use the provided [`CancellationToken`](../interfaces/codearts_plugin_.CancellationToken.md). Note that currently only `ProgressLocation.Notification` is supporting to show a cancel button to cancel the long running operation. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`R`\>

The thenable the task-callback returned.

#### Defined in

[index.d.ts:10124](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10124)

___

### withScmProgress

▸ **withScmProgress**<`R`\>(`task`): [`Thenable`](../interfaces/Thenable.md)<`R`\>

Show progress in the Source Control viewlet while running the given callback and while
its returned promise isn't resolve or rejected.

**`Deprecated`**

Use `withProgress` instead.

#### Type parameters

| Name |
| :------ |
| `R` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `task` | (`progress`: [`Progress`](../interfaces/codearts_plugin_.Progress.md)<`number`\>) => [`Thenable`](../interfaces/Thenable.md)<`R`\> | A callback returning a promise. Progress increments can be reported with the provided [Progress](../interfaces/codearts_plugin_.Progress.md)-object. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`R`\>

The thenable the task did return.

#### Defined in

[index.d.ts:10103](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L10103)
