**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](_index_d_.md) / ["plugin"](_index_d_._plugin_.md) / window

# Namespace: window

Namespace for dealing with the current window of the editor. That is visible
and active editors, as well as, UI elements to show messages, selections, and
asking for user input.

## Index

### Interfaces

* [CustomizableDialog](../interfaces/_index_d_._plugin_.window.customizabledialog.md)
* [CustomizableDialogEvent](../interfaces/_index_d_._plugin_.window.customizabledialogevent.md)
* [CustomizableDialogOptions](../interfaces/_index_d_._plugin_.window.customizabledialogoptions.md)
* [DialogButton](../interfaces/_index_d_._plugin_.window.dialogbutton.md)
* [DialogControlElement](../interfaces/_index_d_._plugin_.window.dialogcontrolelement.md)

### Variables

* [activeColorTheme](_index_d_._plugin_.window.md#activecolortheme)
* [activeTerminal](_index_d_._plugin_.window.md#activeterminal)
* [activeTextEditor](_index_d_._plugin_.window.md#activetexteditor)
* [onDidChangeActiveColorTheme](_index_d_._plugin_.window.md#ondidchangeactivecolortheme)
* [onDidChangeActiveTerminal](_index_d_._plugin_.window.md#ondidchangeactiveterminal)
* [onDidChangeActiveTextEditor](_index_d_._plugin_.window.md#ondidchangeactivetexteditor)
* [onDidChangeTextEditorOptions](_index_d_._plugin_.window.md#ondidchangetexteditoroptions)
* [onDidChangeTextEditorSelection](_index_d_._plugin_.window.md#ondidchangetexteditorselection)
* [onDidChangeTextEditorViewColumn](_index_d_._plugin_.window.md#ondidchangetexteditorviewcolumn)
* [onDidChangeTextEditorVisibleRanges](_index_d_._plugin_.window.md#ondidchangetexteditorvisibleranges)
* [onDidChangeVisibleTextEditors](_index_d_._plugin_.window.md#ondidchangevisibletexteditors)
* [onDidChangeWindowState](_index_d_._plugin_.window.md#ondidchangewindowstate)
* [onDidCloseTerminal](_index_d_._plugin_.window.md#ondidcloseterminal)
* [onDidOpenTerminal](_index_d_._plugin_.window.md#ondidopenterminal)
* [state](_index_d_._plugin_.window.md#state)
* [terminals](_index_d_._plugin_.window.md#terminals)
* [visibleTextEditors](_index_d_._plugin_.window.md#visibletexteditors)

### Functions

* [createCloudWebviewPanel](_index_d_._plugin_.window.md#createcloudwebviewpanel)
* [createCustomizableDialog](_index_d_._plugin_.window.md#createcustomizabledialog)
* [createInputBox](_index_d_._plugin_.window.md#createinputbox)
* [createOutputChannel](_index_d_._plugin_.window.md#createoutputchannel)
* [createQuickPick](_index_d_._plugin_.window.md#createquickpick)
* [createStatusBarItem](_index_d_._plugin_.window.md#createstatusbaritem)
* [createTerminal](_index_d_._plugin_.window.md#createterminal)
* [createTextEditorDecorationType](_index_d_._plugin_.window.md#createtexteditordecorationtype)
* [createTreeView](_index_d_._plugin_.window.md#createtreeview)
* [createWebviewPanel](_index_d_._plugin_.window.md#createwebviewpanel)
* [registerCustomEditorProvider](_index_d_._plugin_.window.md#registercustomeditorprovider)
* [registerFileDecorationProvider](_index_d_._plugin_.window.md#registerfiledecorationprovider)
* [registerTerminalLinkProvider](_index_d_._plugin_.window.md#registerterminallinkprovider)
* [registerTreeDataProvider](_index_d_._plugin_.window.md#registertreedataprovider)
* [registerUriHandler](_index_d_._plugin_.window.md#registerurihandler)
* [registerWebviewAsPluginPage](_index_d_._plugin_.window.md#registerwebviewaspluginpage)
* [registerWebviewPanelSerializer](_index_d_._plugin_.window.md#registerwebviewpanelserializer)
* [registerWebviewViewProvider](_index_d_._plugin_.window.md#registerwebviewviewprovider)
* [setStatusBarMessage](_index_d_._plugin_.window.md#setstatusbarmessage)
* [showErrorMessage](_index_d_._plugin_.window.md#showerrormessage)
* [showInformationMessage](_index_d_._plugin_.window.md#showinformationmessage)
* [showInputBox](_index_d_._plugin_.window.md#showinputbox)
* [showOpenDialog](_index_d_._plugin_.window.md#showopendialog)
* [showQuickPick](_index_d_._plugin_.window.md#showquickpick)
* [showSaveDialog](_index_d_._plugin_.window.md#showsavedialog)
* [showTextDocument](_index_d_._plugin_.window.md#showtextdocument)
* [showWarningMessage](_index_d_._plugin_.window.md#showwarningmessage)
* [showWorkspaceFolderPick](_index_d_._plugin_.window.md#showworkspacefolderpick)
* [withProgress](_index_d_._plugin_.window.md#withprogress)
* [withScmProgress](_index_d_._plugin_.window.md#withscmprogress)

## Variables

### activeColorTheme

• `Let` **activeColorTheme**: [ColorTheme](../interfaces/_index_d_._plugin_.colortheme.md)

*Defined in [index.d.ts:9007](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9007)*

The currently active color theme as configured in the settings. The active
theme can be changed via the `workbench.colorTheme` setting.

___

### activeTerminal

• `Const` **activeTerminal**: [Terminal](../interfaces/_index_d_._plugin_.terminal.md) \| undefined

*Defined in [index.d.ts:8300](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8300)*

The currently active terminal or `undefined`. The active terminal is the one that
currently has focus or most recently had focus.

___

### activeTextEditor

• `Let` **activeTextEditor**: [TextEditor](../interfaces/_index_d_._plugin_.texteditor.md) \| undefined

*Defined in [index.d.ts:8251](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8251)*

The currently active editor or `undefined`. The active editor is the one
that currently has focus or, when none has focus, the one that has changed
input most recently.

___

### onDidChangeActiveColorTheme

• `Const` **onDidChangeActiveColorTheme**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[ColorTheme](../interfaces/_index_d_._plugin_.colortheme.md)>

*Defined in [index.d.ts:9012](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9012)*

An [event](#Event) which fires when the active color theme is changed or has changes.

___

### onDidChangeActiveTerminal

• `Const` **onDidChangeActiveTerminal**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[Terminal](../interfaces/_index_d_._plugin_.terminal.md) \| undefined>

*Defined in [index.d.ts:8307](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8307)*

An [event](#Event) which fires when the [active terminal](#window.activeTerminal)
has changed. *Note* that the event also fires when the active terminal changes
to `undefined`.

___

### onDidChangeActiveTextEditor

• `Const` **onDidChangeActiveTextEditor**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[TextEditor](../interfaces/_index_d_._plugin_.texteditor.md) \| undefined>

*Defined in [index.d.ts:8263](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8263)*

An [event](#Event) which fires when the [active editor](#window.activeTextEditor)
has changed. *Note* that the event also fires when the active editor changes
to `undefined`.

___

### onDidChangeTextEditorOptions

• `Const` **onDidChangeTextEditorOptions**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[TextEditorOptionsChangeEvent](../interfaces/_index_d_._plugin_.texteditoroptionschangeevent.md)>

*Defined in [index.d.ts:8284](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8284)*

An [event](#Event) which fires when the options of an editor have changed.

___

### onDidChangeTextEditorSelection

• `Const` **onDidChangeTextEditorSelection**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[TextEditorSelectionChangeEvent](../interfaces/_index_d_._plugin_.texteditorselectionchangeevent.md)>

*Defined in [index.d.ts:8274](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8274)*

An [event](#Event) which fires when the selection in an editor has changed.

___

### onDidChangeTextEditorViewColumn

• `Const` **onDidChangeTextEditorViewColumn**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[TextEditorViewColumnChangeEvent](../interfaces/_index_d_._plugin_.texteditorviewcolumnchangeevent.md)>

*Defined in [index.d.ts:8289](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8289)*

An [event](#Event) which fires when the view column of an editor has changed.

___

### onDidChangeTextEditorVisibleRanges

• `Const` **onDidChangeTextEditorVisibleRanges**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[TextEditorVisibleRangesChangeEvent](../interfaces/_index_d_._plugin_.texteditorvisiblerangeschangeevent.md)>

*Defined in [index.d.ts:8279](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8279)*

An [event](#Event) which fires when the visible ranges of an editor has changed.

___

### onDidChangeVisibleTextEditors

• `Const` **onDidChangeVisibleTextEditors**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[TextEditor](../interfaces/_index_d_._plugin_.texteditor.md)[]>

*Defined in [index.d.ts:8269](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8269)*

An [event](#Event) which fires when the array of [visible editors](#window.visibleTextEditors)
has changed.

___

### onDidChangeWindowState

• `Const` **onDidChangeWindowState**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[WindowState](../interfaces/_index_d_._plugin_.windowstate.md)>

*Defined in [index.d.ts:8329](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8329)*

An [event](#Event) which fires when the focus state of the current window
changes. The value of the event represents whether the window is focused.

___

### onDidCloseTerminal

• `Const` **onDidCloseTerminal**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[Terminal](../interfaces/_index_d_._plugin_.terminal.md)>

*Defined in [index.d.ts:8318](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8318)*

An [event](#Event) which fires when a terminal is disposed.

___

### onDidOpenTerminal

• `Const` **onDidOpenTerminal**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[Terminal](../interfaces/_index_d_._plugin_.terminal.md)>

*Defined in [index.d.ts:8313](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8313)*

An [event](#Event) which fires when a terminal has been created, either through the
[createTerminal](#window.createTerminal) API or commands.

___

### state

• `Const` **state**: [WindowState](../interfaces/_index_d_._plugin_.windowstate.md)

*Defined in [index.d.ts:8323](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8323)*

Represents the current window's state.

___

### terminals

• `Const` **terminals**: ReadonlyArray\<[Terminal](../interfaces/_index_d_._plugin_.terminal.md)>

*Defined in [index.d.ts:8294](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8294)*

The currently opened terminals or an empty array.

___

### visibleTextEditors

• `Let` **visibleTextEditors**: [TextEditor](../interfaces/_index_d_._plugin_.texteditor.md)[]

*Defined in [index.d.ts:8256](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8256)*

The currently visible editors or an empty array.

## Functions

### createCloudWebviewPanel

▸ **createCloudWebviewPanel**(`viewType`: string, `title`: string, `showOptions`: [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md) \| { area: string ; preserveFocus?: boolean ; viewColumn: [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md)  }, `options?`: [WebviewPanelOptions](../interfaces/_index_d_._plugin_.webviewpaneloptions.md) & [WebviewOptions](../interfaces/_index_d_._plugin_.webviewoptions.md)): [WebviewPanel](../interfaces/_index_d_._plugin_.webviewpanel.md)

*Defined in [index.d.ts:8641](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8641)*

Create and show a new webview panel.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`viewType` | string | Identifies the type of the webview panel. |
`title` | string | Title of the panel. |
`showOptions` | [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md) \| { area: string ; preserveFocus?: boolean ; viewColumn: [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md)  } | where webview panel will be reside. If preserveFocus is set, the new webview will not take focus. |
`options?` | [WebviewPanelOptions](../interfaces/_index_d_._plugin_.webviewpaneloptions.md) & [WebviewOptions](../interfaces/_index_d_._plugin_.webviewoptions.md) | Settings for the new panel.  |

**Returns:** [WebviewPanel](../interfaces/_index_d_._plugin_.webviewpanel.md)

New webview panel.

___

### createCustomizableDialog

▸ **createCustomizableDialog**(`options`: [CustomizableDialogOptions](../interfaces/_index_d_._plugin_.window.customizabledialogoptions.md)): Promise\<[CustomizableDialog](../interfaces/_index_d_._plugin_.window.customizabledialog.md)>

*Defined in [index.d.ts:8651](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8651)*

Create and show a new dialog with a iframe inside.
You can set the contents of the dialog box as you like.

#### Parameters:

Name | Type |
------ | ------ |
`options` | [CustomizableDialogOptions](../interfaces/_index_d_._plugin_.window.customizabledialogoptions.md) |

**Returns:** Promise\<[CustomizableDialog](../interfaces/_index_d_._plugin_.window.customizabledialog.md)>

Dialog operations object.

___

### createInputBox

▸ **createInputBox**(): [InputBox](../interfaces/_index_d_._plugin_.inputbox.md)

*Defined in [index.d.ts:8610](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8610)*

Creates a [InputBox](#InputBox) to let the user enter some text input.

Note that in many cases the more convenient [window.showInputBox](#window.showInputBox)
is easier to use. [window.createInputBox](#window.createInputBox) should be used
when [window.showInputBox](#window.showInputBox) does not offer the required flexibility.

**Returns:** [InputBox](../interfaces/_index_d_._plugin_.inputbox.md)

A new [InputBox](#InputBox).

___

### createOutputChannel

▸ **createOutputChannel**(`name`: string): [OutputChannel](../interfaces/_index_d_._plugin_.outputchannel.md)

*Defined in [index.d.ts:8617](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8617)*

Creates a new [output channel](#OutputChannel) with the given name.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`name` | string | Human-readable string which will be used to represent the channel in the UI.  |

**Returns:** [OutputChannel](../interfaces/_index_d_._plugin_.outputchannel.md)

___

### createQuickPick

▸ **createQuickPick**\<T>(): [QuickPick](../interfaces/_index_d_._plugin_.quickpick.md)\<T>

*Defined in [index.d.ts:8599](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8599)*

Creates a [QuickPick](#QuickPick) to let the user pick an item from a list
of items of type T.

Note that in many cases the more convenient [window.showQuickPick](#window.showQuickPick)
is easier to use. [window.createQuickPick](#window.createQuickPick) should be used
when [window.showQuickPick](#window.showQuickPick) does not offer the required flexibility.

#### Type parameters:

Name | Type |
------ | ------ |
`T` | [QuickPickItem](../interfaces/_index_d_._plugin_.quickpickitem.md) |

**Returns:** [QuickPick](../interfaces/_index_d_._plugin_.quickpick.md)\<T>

A new [QuickPick](#QuickPick).

___

### createStatusBarItem

▸ **createStatusBarItem**(`alignment?`: [StatusBarAlignment](../enums/_index_d_._plugin_.statusbaralignment.md), `priority?`: number): [StatusBarItem](../interfaces/_index_d_._plugin_.statusbaritem.md)

*Defined in [index.d.ts:8821](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8821)*

Creates a status bar [item](#StatusBarItem).

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`alignment?` | [StatusBarAlignment](../enums/_index_d_._plugin_.statusbaralignment.md) | The alignment of the item. |
`priority?` | number | The priority of the item. Higher values mean the item should be shown more to the left. |

**Returns:** [StatusBarItem](../interfaces/_index_d_._plugin_.statusbaritem.md)

A new status bar item.

___

### createTerminal

▸ **createTerminal**(`name?`: string, `shellPath?`: string, `shellArgs?`: string[] \| string): [Terminal](../interfaces/_index_d_._plugin_.terminal.md)

*Defined in [index.d.ts:8835](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8835)*

Creates a [Terminal](#Terminal) with a backing shell process. The cwd of the terminal will be the workspace
directory if it exists.

**`throws`** When running in an environment where a new process cannot be started.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`name?` | string | Optional human-readable string which will be used to represent the terminal in the UI. |
`shellPath?` | string | Optional path to a custom shell executable to be used in the terminal. |
`shellArgs?` | string[] \| string | Optional args for the custom shell executable. A string can be used on Windows only which allows specifying shell args in [command-line format](https://msdn.microsoft.com/en-au/08dfcab2-eb6e-49a4-80eb-87d4076c98c6). |

**Returns:** [Terminal](../interfaces/_index_d_._plugin_.terminal.md)

A new Terminal.

▸ **createTerminal**(`options`: [TerminalOptions](../interfaces/_index_d_._plugin_.terminaloptions.md)): [Terminal](../interfaces/_index_d_._plugin_.terminal.md)

*Defined in [index.d.ts:8844](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8844)*

Creates a [Terminal](#Terminal) with a backing shell process.

**`throws`** When running in an environment where a new process cannot be started.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`options` | [TerminalOptions](../interfaces/_index_d_._plugin_.terminaloptions.md) | A TerminalOptions object describing the characteristics of the new terminal. |

**Returns:** [Terminal](../interfaces/_index_d_._plugin_.terminal.md)

A new Terminal.

▸ **createTerminal**(`options`: [ExtensionTerminalOptions](../interfaces/_index_d_._plugin_.extensionterminaloptions.md)): [Terminal](../interfaces/_index_d_._plugin_.terminal.md)

*Defined in [index.d.ts:8853](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8853)*

Creates a [Terminal](#Terminal) where an extension controls its input and output.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`options` | [ExtensionTerminalOptions](../interfaces/_index_d_._plugin_.extensionterminaloptions.md) | An [ExtensionTerminalOptions](#ExtensionTerminalOptions) object describing the characteristics of the new terminal. |

**Returns:** [Terminal](../interfaces/_index_d_._plugin_.terminal.md)

A new Terminal.

___

### createTextEditorDecorationType

▸ **createTextEditorDecorationType**(`options`: [DecorationRenderOptions](../interfaces/_index_d_._plugin_.decorationrenderoptions.md)): [TextEditorDecorationType](../interfaces/_index_d_._plugin_.texteditordecorationtype.md)

*Defined in [index.d.ts:8371](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8371)*

Create a TextEditorDecorationType that can be used to add decorations to text editors.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`options` | [DecorationRenderOptions](../interfaces/_index_d_._plugin_.decorationrenderoptions.md) | Rendering options for the decoration type. |

**Returns:** [TextEditorDecorationType](../interfaces/_index_d_._plugin_.texteditordecorationtype.md)

A new decoration type instance.

___

### createTreeView

▸ **createTreeView**\<T>(`viewId`: string, `options`: [TreeViewOptions](../interfaces/_index_d_._plugin_.treeviewoptions.md)\<T>): [TreeView](../interfaces/_index_d_._plugin_.treeview.md)\<T>

*Defined in [index.d.ts:8872](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8872)*

Create a [TreeView](#TreeView) for the view contributed using the extension point `views`.

#### Type parameters:

Name |
------ |
`T` |

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`viewId` | string | Id of the view contributed using the extension point `views`. |
`options` | [TreeViewOptions](../interfaces/_index_d_._plugin_.treeviewoptions.md)\<T> | Options for creating the [TreeView](#TreeView) |

**Returns:** [TreeView](../interfaces/_index_d_._plugin_.treeview.md)\<T>

a [TreeView](#TreeView).

___

### createWebviewPanel

▸ **createWebviewPanel**(`viewType`: string, `title`: string, `showOptions`: [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md) \| { preserveFocus?: boolean ; viewColumn: [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md)  }, `options?`: [WebviewPanelOptions](../interfaces/_index_d_._plugin_.webviewpaneloptions.md) & [WebviewOptions](../interfaces/_index_d_._plugin_.webviewoptions.md)): [WebviewPanel](../interfaces/_index_d_._plugin_.webviewpanel.md)

*Defined in [index.d.ts:8629](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8629)*

Create and show a new webview panel.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`viewType` | string | Identifies the type of the webview panel. |
`title` | string | Title of the panel. |
`showOptions` | [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md) \| { preserveFocus?: boolean ; viewColumn: [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md)  } | Where to show the webview in the editor. If preserveFocus is set, the new webview will not take focus. |
`options?` | [WebviewPanelOptions](../interfaces/_index_d_._plugin_.webviewpaneloptions.md) & [WebviewOptions](../interfaces/_index_d_._plugin_.webviewoptions.md) | Settings for the new panel.  |

**Returns:** [WebviewPanel](../interfaces/_index_d_._plugin_.webviewpanel.md)

New webview panel.

___

### registerCustomEditorProvider

▸ **registerCustomEditorProvider**(`viewType`: string, `provider`: [CustomTextEditorProvider](../interfaces/_index_d_._plugin_.customtexteditorprovider.md) \| [CustomReadonlyEditorProvider](../interfaces/_index_d_._plugin_.customreadonlyeditorprovider.md) \| [CustomEditorProvider](../interfaces/_index_d_._plugin_.customeditorprovider.md), `options?`: { supportsMultipleEditorsPerDocument?: boolean ; webviewOptions?: [WebviewPanelOptions](../interfaces/_index_d_._plugin_.webviewpaneloptions.md)  }): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:8965](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8965)*

Register a provider for custom editors for the `viewType` contributed by the `customEditors` extension point.

When a custom editor is opened, VS Code fires an `onCustomEditor:viewType` activation event. Your extension
must register a [`CustomTextEditorProvider`](#CustomTextEditorProvider), [`CustomReadonlyEditorProvider`](#CustomReadonlyEditorProvider),
[`CustomEditorProvider`](#CustomEditorProvider)for `viewType` as part of activation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`viewType` | string | Unique identifier for the custom editor provider. This should match the `viewType` from the   `customEditors` contribution point. |
`provider` | [CustomTextEditorProvider](../interfaces/_index_d_._plugin_.customtexteditorprovider.md) \| [CustomReadonlyEditorProvider](../interfaces/_index_d_._plugin_.customreadonlyeditorprovider.md) \| [CustomEditorProvider](../interfaces/_index_d_._plugin_.customeditorprovider.md) | Provider that resolves custom editors. |
`options?` | { supportsMultipleEditorsPerDocument?: boolean ; webviewOptions?: [WebviewPanelOptions](../interfaces/_index_d_._plugin_.webviewpaneloptions.md)  } | Options for the provider.  |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

Disposable that unregisters the provider.

___

### registerFileDecorationProvider

▸ **registerFileDecorationProvider**(`provider`: [FileDecorationProvider](../interfaces/_index_d_._plugin_.filedecorationprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:9001](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9001)*

Register a file decoration provider.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`provider` | [FileDecorationProvider](../interfaces/_index_d_._plugin_.filedecorationprovider.md) | A [FileDecorationProvider](#FileDecorationProvider). |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters the provider.

___

### registerTerminalLinkProvider

▸ **registerTerminalLinkProvider**(`provider`: [TerminalLinkProvider](../interfaces/_index_d_._plugin_.terminallinkprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:8993](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8993)*

Register provider that enables the detection and handling of links within the terminal.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`provider` | [TerminalLinkProvider](../interfaces/_index_d_._plugin_.terminallinkprovider.md) | The provider that provides the terminal links. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

Disposable that unregisters the provider.

___

### registerTreeDataProvider

▸ **registerTreeDataProvider**\<T>(`viewId`: string, `treeDataProvider`: [TreeDataProvider](../interfaces/_index_d_._plugin_.treedataprovider.md)\<T>): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:8864](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8864)*

Register a [TreeDataProvider](#TreeDataProvider) for the view contributed using the extension point `views`.
This will allow you to contribute data to the [TreeView](#TreeView) and update if the data changes.

**Note:** To get access to the [TreeView](#TreeView) and perform operations on it, use [createTreeView](#window.createTreeView).

#### Type parameters:

Name |
------ |
`T` |

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`viewId` | string | Id of the view contributed using the extension point `views`. |
`treeDataProvider` | [TreeDataProvider](../interfaces/_index_d_._plugin_.treedataprovider.md)\<T> | A [TreeDataProvider](#TreeDataProvider) that provides tree data for the view  |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

___

### registerUriHandler

▸ **registerUriHandler**(`handler`: [UriHandler](../interfaces/_index_d_._plugin_.urihandler.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:8895](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8895)*

Registers a [uri handler](#UriHandler) capable of handling system-wide [uris](#Uri).
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

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`handler` | [UriHandler](../interfaces/_index_d_._plugin_.urihandler.md) | The uri handler to register for this extension.  |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

___

### registerWebviewAsPluginPage

▸ **registerWebviewAsPluginPage**(`viewType`: string): void

*Defined in [index.d.ts:8915](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8915)*

Only registers a webview panel.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`viewType` | string | Type of the webview panel.  |

**Returns:** void

___

### registerWebviewPanelSerializer

▸ **registerWebviewPanelSerializer**(`viewType`: string, `serializer`: [WebviewPanelSerializer](../interfaces/_index_d_._plugin_.webviewpanelserializer.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:8908](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8908)*

Registers a webview panel serializer.

Extensions that support reviving should have an `"onWebviewPanel:viewType"` activation event and
make sure that [registerWebviewPanelSerializer](#registerWebviewPanelSerializer) is called during activation.

Only a single serializer may be registered at a time for a given `viewType`.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`viewType` | string | Type of the webview panel that can be serialized. |
`serializer` | [WebviewPanelSerializer](../interfaces/_index_d_._plugin_.webviewpanelserializer.md) | Webview serializer.  |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

___

### registerWebviewViewProvider

▸ **registerWebviewViewProvider**(`viewId`: string, `provider`: [WebviewViewProvider](../interfaces/_index_d_._plugin_.webviewviewprovider.md), `options?`: { webviewOptions?: { retainContextWhenHidden?: boolean  }  }): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:8926](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8926)*

Register a new provider for webview views.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`viewId` | string | Unique id of the view. This should match the `id` from the   `views` contribution in the package.json. |
`provider` | [WebviewViewProvider](../interfaces/_index_d_._plugin_.webviewviewprovider.md) | Provider for the webview views.  |
`options?` | { webviewOptions?: { retainContextWhenHidden?: boolean  }  } | - |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

Disposable that unregisters the provider.

___

### setStatusBarMessage

▸ **setStatusBarMessage**(`text`: string, `hideAfterTimeout`: number): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:8757](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8757)*

Set a message to the status bar. This is a short hand for the more powerful
status bar [items](#window.createStatusBarItem).

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`text` | string | The message to show, supports icon substitution as in status bar [items](#StatusBarItem.text). |
`hideAfterTimeout` | number | Timeout in milliseconds after which the message will be disposed. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A disposable which hides the status bar message.

▸ **setStatusBarMessage**(`text`: string, `hideWhenDone`: [Thenable](../interfaces/_index_d_.thenable.md)\<any>): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:8767](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8767)*

Set a message to the status bar. This is a short hand for the more powerful
status bar [items](#window.createStatusBarItem).

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`text` | string | The message to show, supports icon substitution as in status bar [items](#StatusBarItem.text). |
`hideWhenDone` | [Thenable](../interfaces/_index_d_.thenable.md)\<any> | Thenable on which completion (resolve or reject) the message will be disposed. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A disposable which hides the status bar message.

▸ **setStatusBarMessage**(`text`: string): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:8779](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8779)*

Set a message to the status bar. This is a short hand for the more powerful
status bar [items](#window.createStatusBarItem).

*Note* that status bar messages stack and that they must be disposed when no
longer used.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`text` | string | The message to show, supports icon substitution as in status bar [items](#StatusBarItem.text). |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A disposable which hides the status bar message.

___

### showErrorMessage

▸ **showErrorMessage**(`message`: string, ...`items`: string[]): [Thenable](../interfaces/_index_d_.thenable.md)\<string \| undefined>

*Defined in [index.d.ts:8472](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8472)*

Show an error message.

**`see`** [showInformationMessage](#window.showInformationMessage)

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`message` | string | The message to show. |
`...items` | string[] | A set of items that will be rendered as actions in the message. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<string \| undefined>

A thenable that resolves to the selected item or `undefined` when being dismissed.

▸ **showErrorMessage**(`message`: string, `options`: [MessageOptions](../interfaces/_index_d_._plugin_.messageoptions.md), ...`items`: string[]): [Thenable](../interfaces/_index_d_.thenable.md)\<string \| undefined>

*Defined in [index.d.ts:8484](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8484)*

Show an error message.

**`see`** [showInformationMessage](#window.showInformationMessage)

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`message` | string | The message to show. |
`options` | [MessageOptions](../interfaces/_index_d_._plugin_.messageoptions.md) | Configures the behaviour of the message. |
`...items` | string[] | A set of items that will be rendered as actions in the message. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<string \| undefined>

A thenable that resolves to the selected item or `undefined` when being dismissed.

▸ **showErrorMessage**\<T>(`message`: string, ...`items`: T[]): [Thenable](../interfaces/_index_d_.thenable.md)\<T \| undefined>

*Defined in [index.d.ts:8495](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8495)*

Show an error message.

**`see`** [showInformationMessage](#window.showInformationMessage)

#### Type parameters:

Name | Type |
------ | ------ |
`T` | [MessageItem](../interfaces/_index_d_._plugin_.messageitem.md) |

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`message` | string | The message to show. |
`...items` | T[] | A set of items that will be rendered as actions in the message. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<T \| undefined>

A thenable that resolves to the selected item or `undefined` when being dismissed.

▸ **showErrorMessage**\<T>(`message`: string, `options`: [MessageOptions](../interfaces/_index_d_._plugin_.messageoptions.md), ...`items`: T[]): [Thenable](../interfaces/_index_d_.thenable.md)\<T \| undefined>

*Defined in [index.d.ts:8507](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8507)*

Show an error message.

**`see`** [showInformationMessage](#window.showInformationMessage)

#### Type parameters:

Name | Type |
------ | ------ |
`T` | [MessageItem](../interfaces/_index_d_._plugin_.messageitem.md) |

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`message` | string | The message to show. |
`options` | [MessageOptions](../interfaces/_index_d_._plugin_.messageoptions.md) | Configures the behaviour of the message. |
`...items` | T[] | A set of items that will be rendered as actions in the message. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<T \| undefined>

A thenable that resolves to the selected item or `undefined` when being dismissed.

___

### showInformationMessage

▸ **showInformationMessage**(`message`: string, ...`items`: string[]): [Thenable](../interfaces/_index_d_.thenable.md)\<string \| undefined>

*Defined in [index.d.ts:8381](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8381)*

Show an information message to users. Optionally provide an array of items which will be presented as
clickable buttons.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`message` | string | The message to show. |
`...items` | string[] | A set of items that will be rendered as actions in the message. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<string \| undefined>

A thenable that resolves to the selected item or `undefined` when being dismissed.

▸ **showInformationMessage**(`message`: string, `options`: [MessageOptions](../interfaces/_index_d_._plugin_.messageoptions.md), ...`items`: string[]): [Thenable](../interfaces/_index_d_.thenable.md)\<string \| undefined>

*Defined in [index.d.ts:8392](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8392)*

Show an information message to users. Optionally provide an array of items which will be presented as
clickable buttons.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`message` | string | The message to show. |
`options` | [MessageOptions](../interfaces/_index_d_._plugin_.messageoptions.md) | Configures the behaviour of the message. |
`...items` | string[] | A set of items that will be rendered as actions in the message. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<string \| undefined>

A thenable that resolves to the selected item or `undefined` when being dismissed.

▸ **showInformationMessage**\<T>(`message`: string, ...`items`: T[]): [Thenable](../interfaces/_index_d_.thenable.md)\<T \| undefined>

*Defined in [index.d.ts:8403](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8403)*

Show an information message.

**`see`** [showInformationMessage](#window.showInformationMessage)

#### Type parameters:

Name | Type |
------ | ------ |
`T` | [MessageItem](../interfaces/_index_d_._plugin_.messageitem.md) |

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`message` | string | The message to show. |
`...items` | T[] | A set of items that will be rendered as actions in the message. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<T \| undefined>

A thenable that resolves to the selected item or `undefined` when being dismissed.

▸ **showInformationMessage**\<T>(`message`: string, `options`: [MessageOptions](../interfaces/_index_d_._plugin_.messageoptions.md), ...`items`: T[]): [Thenable](../interfaces/_index_d_.thenable.md)\<T \| undefined>

*Defined in [index.d.ts:8415](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8415)*

Show an information message.

**`see`** [showInformationMessage](#window.showInformationMessage)

#### Type parameters:

Name | Type |
------ | ------ |
`T` | [MessageItem](../interfaces/_index_d_._plugin_.messageitem.md) |

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`message` | string | The message to show. |
`options` | [MessageOptions](../interfaces/_index_d_._plugin_.messageoptions.md) | Configures the behaviour of the message. |
`...items` | T[] | A set of items that will be rendered as actions in the message. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<T \| undefined>

A thenable that resolves to the selected item or `undefined` when being dismissed.

___

### showInputBox

▸ **showInputBox**(`options?`: [InputBoxOptions](../interfaces/_index_d_._plugin_.inputboxoptions.md), `token?`: [CancellationToken](../interfaces/_index_d_._plugin_.cancellationtoken.md)): [Thenable](../interfaces/_index_d_.thenable.md)\<string \| undefined>

*Defined in [index.d.ts:8587](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8587)*

Opens an input box to ask the user for input.

The returned value will be `undefined` if the input box was canceled (e.g. pressing ESC). Otherwise the
returned value will be the string typed by the user or an empty string if the user did not type
anything but dismissed the input box with OK.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`options?` | [InputBoxOptions](../interfaces/_index_d_._plugin_.inputboxoptions.md) | Configures the behavior of the input box. |
`token?` | [CancellationToken](../interfaces/_index_d_._plugin_.cancellationtoken.md) | A token that can be used to signal cancellation. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<string \| undefined>

A promise that resolves to a string the user provided or to `undefined` in case of dismissal.

___

### showOpenDialog

▸ **showOpenDialog**(`options?`: [OpenDialogOptions](../interfaces/_index_d_._plugin_.opendialogoptions.md)): [Thenable](../interfaces/_index_d_.thenable.md)\<[Uri](../classes/_index_d_._plugin_.uri.md)[] \| undefined>

*Defined in [index.d.ts:8565](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8565)*

Shows a file open dialog to the user which allows to select a file
for opening-purposes.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`options?` | [OpenDialogOptions](../interfaces/_index_d_._plugin_.opendialogoptions.md) | Options that control the dialog. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<[Uri](../classes/_index_d_._plugin_.uri.md)[] \| undefined>

A promise that resolves to the selected resources or `undefined`.

___

### showQuickPick

▸ **showQuickPick**(`items`: string[] \| [Thenable](../interfaces/_index_d_.thenable.md)\<string[]>, `options`: [QuickPickOptions](../interfaces/_index_d_._plugin_.quickpickoptions.md) & { canPickMany: true  }, `token?`: [CancellationToken](../interfaces/_index_d_._plugin_.cancellationtoken.md)): [Thenable](../interfaces/_index_d_.thenable.md)\<string[] \| undefined>

*Defined in [index.d.ts:8517](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8517)*

Shows a selection list allowing multiple selections.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`items` | string[] \| [Thenable](../interfaces/_index_d_.thenable.md)\<string[]> | An array of strings, or a promise that resolves to an array of strings. |
`options` | [QuickPickOptions](../interfaces/_index_d_._plugin_.quickpickoptions.md) & { canPickMany: true  } | Configures the behavior of the selection list. |
`token?` | [CancellationToken](../interfaces/_index_d_._plugin_.cancellationtoken.md) | A token that can be used to signal cancellation. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<string[] \| undefined>

A promise that resolves to the selected items or `undefined`.

▸ **showQuickPick**(`items`: string[] \| [Thenable](../interfaces/_index_d_.thenable.md)\<string[]>, `options?`: [QuickPickOptions](../interfaces/_index_d_._plugin_.quickpickoptions.md), `token?`: [CancellationToken](../interfaces/_index_d_._plugin_.cancellationtoken.md)): [Thenable](../interfaces/_index_d_.thenable.md)\<string \| undefined>

*Defined in [index.d.ts:8527](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8527)*

Shows a selection list.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`items` | string[] \| [Thenable](../interfaces/_index_d_.thenable.md)\<string[]> | An array of strings, or a promise that resolves to an array of strings. |
`options?` | [QuickPickOptions](../interfaces/_index_d_._plugin_.quickpickoptions.md) | Configures the behavior of the selection list. |
`token?` | [CancellationToken](../interfaces/_index_d_._plugin_.cancellationtoken.md) | A token that can be used to signal cancellation. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<string \| undefined>

A promise that resolves to the selection or `undefined`.

▸ **showQuickPick**\<T>(`items`: T[] \| [Thenable](../interfaces/_index_d_.thenable.md)\<T[]>, `options`: [QuickPickOptions](../interfaces/_index_d_._plugin_.quickpickoptions.md) & { canPickMany: true  }, `token?`: [CancellationToken](../interfaces/_index_d_._plugin_.cancellationtoken.md)): [Thenable](../interfaces/_index_d_.thenable.md)\<T[] \| undefined>

*Defined in [index.d.ts:8537](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8537)*

Shows a selection list allowing multiple selections.

#### Type parameters:

Name | Type |
------ | ------ |
`T` | [QuickPickItem](../interfaces/_index_d_._plugin_.quickpickitem.md) |

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`items` | T[] \| [Thenable](../interfaces/_index_d_.thenable.md)\<T[]> | An array of items, or a promise that resolves to an array of items. |
`options` | [QuickPickOptions](../interfaces/_index_d_._plugin_.quickpickoptions.md) & { canPickMany: true  } | Configures the behavior of the selection list. |
`token?` | [CancellationToken](../interfaces/_index_d_._plugin_.cancellationtoken.md) | A token that can be used to signal cancellation. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<T[] \| undefined>

A promise that resolves to the selected items or `undefined`.

▸ **showQuickPick**\<T>(`items`: T[] \| [Thenable](../interfaces/_index_d_.thenable.md)\<T[]>, `options?`: [QuickPickOptions](../interfaces/_index_d_._plugin_.quickpickoptions.md), `token?`: [CancellationToken](../interfaces/_index_d_._plugin_.cancellationtoken.md)): [Thenable](../interfaces/_index_d_.thenable.md)\<T \| undefined>

*Defined in [index.d.ts:8547](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8547)*

Shows a selection list.

#### Type parameters:

Name | Type |
------ | ------ |
`T` | [QuickPickItem](../interfaces/_index_d_._plugin_.quickpickitem.md) |

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`items` | T[] \| [Thenable](../interfaces/_index_d_.thenable.md)\<T[]> | An array of items, or a promise that resolves to an array of items. |
`options?` | [QuickPickOptions](../interfaces/_index_d_._plugin_.quickpickoptions.md) | Configures the behavior of the selection list. |
`token?` | [CancellationToken](../interfaces/_index_d_._plugin_.cancellationtoken.md) | A token that can be used to signal cancellation. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<T \| undefined>

A promise that resolves to the selected item or `undefined`.

___

### showSaveDialog

▸ **showSaveDialog**(`options?`: [SaveDialogOptions](../interfaces/_index_d_._plugin_.savedialogoptions.md)): [Thenable](../interfaces/_index_d_.thenable.md)\<[Uri](../classes/_index_d_._plugin_.uri.md) \| undefined>

*Defined in [index.d.ts:8574](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8574)*

Shows a file save dialog to the user which allows to select a file
for saving-purposes.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`options?` | [SaveDialogOptions](../interfaces/_index_d_._plugin_.savedialogoptions.md) | Options that control the dialog. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<[Uri](../classes/_index_d_._plugin_.uri.md) \| undefined>

A promise that resolves to the selected resource or `undefined`.

___

### showTextDocument

▸ **showTextDocument**(`document`: [TextDocument](../interfaces/_index_d_._plugin_.textdocument.md), `column?`: [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md), `preserveFocus?`: boolean): [Thenable](../interfaces/_index_d_.thenable.md)\<[TextEditor](../interfaces/_index_d_._plugin_.texteditor.md)>

*Defined in [index.d.ts:8342](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8342)*

Show the given document in a text editor. A [column](#ViewColumn) can be provided
to control where the editor is being shown. Might change the [active editor](#window.activeTextEditor).

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](../interfaces/_index_d_._plugin_.textdocument.md) | A text document to be shown. |
`column?` | [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md) | A view column in which the [editor](#TextEditor) should be shown. The default is the [active](#ViewColumn.Active), other values are adjusted to be `Min(column, columnCount + 1)`, the [active](#ViewColumn.Active)-column is not adjusted. Use [`ViewColumn.Beside`](#ViewColumn.Beside) to open the editor to the side of the currently active one. |
`preserveFocus?` | boolean | When `true` the editor will not take focus. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<[TextEditor](../interfaces/_index_d_._plugin_.texteditor.md)>

A promise that resolves to an [editor](#TextEditor).

▸ **showTextDocument**(`document`: [TextDocument](../interfaces/_index_d_._plugin_.textdocument.md), `options?`: [TextDocumentShowOptions](../interfaces/_index_d_._plugin_.textdocumentshowoptions.md)): [Thenable](../interfaces/_index_d_.thenable.md)\<[TextEditor](../interfaces/_index_d_._plugin_.texteditor.md)>

*Defined in [index.d.ts:8352](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8352)*

Show the given document in a text editor. [Options](#TextDocumentShowOptions) can be provided
to control options of the editor is being shown. Might change the [active editor](#window.activeTextEditor).

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](../interfaces/_index_d_._plugin_.textdocument.md) | A text document to be shown. |
`options?` | [TextDocumentShowOptions](../interfaces/_index_d_._plugin_.textdocumentshowoptions.md) | (#TextDocumentShowOptions) to configure the behavior of showing the [editor](#TextEditor). |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<[TextEditor](../interfaces/_index_d_._plugin_.texteditor.md)>

A promise that resolves to an [editor](#TextEditor).

▸ **showTextDocument**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md), `options?`: [TextDocumentShowOptions](../interfaces/_index_d_._plugin_.textdocumentshowoptions.md)): [Thenable](../interfaces/_index_d_.thenable.md)\<[TextEditor](../interfaces/_index_d_._plugin_.texteditor.md)>

*Defined in [index.d.ts:8363](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8363)*

A short-hand for `openTextDocument(uri).then(document => showTextDocument(document, options))`.

**`see`** [openTextDocument](#openTextDocument)

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | A resource identifier. |
`options?` | [TextDocumentShowOptions](../interfaces/_index_d_._plugin_.textdocumentshowoptions.md) | (#TextDocumentShowOptions) to configure the behavior of showing the [editor](#TextEditor). |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<[TextEditor](../interfaces/_index_d_._plugin_.texteditor.md)>

A promise that resolves to an [editor](#TextEditor).

___

### showWarningMessage

▸ **showWarningMessage**(`message`: string, ...`items`: string[]): [Thenable](../interfaces/_index_d_.thenable.md)\<string \| undefined>

*Defined in [index.d.ts:8426](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8426)*

Show a warning message.

**`see`** [showInformationMessage](#window.showInformationMessage)

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`message` | string | The message to show. |
`...items` | string[] | A set of items that will be rendered as actions in the message. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<string \| undefined>

A thenable that resolves to the selected item or `undefined` when being dismissed.

▸ **showWarningMessage**(`message`: string, `options`: [MessageOptions](../interfaces/_index_d_._plugin_.messageoptions.md), ...`items`: string[]): [Thenable](../interfaces/_index_d_.thenable.md)\<string \| undefined>

*Defined in [index.d.ts:8438](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8438)*

Show a warning message.

**`see`** [showInformationMessage](#window.showInformationMessage)

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`message` | string | The message to show. |
`options` | [MessageOptions](../interfaces/_index_d_._plugin_.messageoptions.md) | Configures the behaviour of the message. |
`...items` | string[] | A set of items that will be rendered as actions in the message. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<string \| undefined>

A thenable that resolves to the selected item or `undefined` when being dismissed.

▸ **showWarningMessage**\<T>(`message`: string, ...`items`: T[]): [Thenable](../interfaces/_index_d_.thenable.md)\<T \| undefined>

*Defined in [index.d.ts:8449](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8449)*

Show a warning message.

**`see`** [showInformationMessage](#window.showInformationMessage)

#### Type parameters:

Name | Type |
------ | ------ |
`T` | [MessageItem](../interfaces/_index_d_._plugin_.messageitem.md) |

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`message` | string | The message to show. |
`...items` | T[] | A set of items that will be rendered as actions in the message. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<T \| undefined>

A thenable that resolves to the selected item or `undefined` when being dismissed.

▸ **showWarningMessage**\<T>(`message`: string, `options`: [MessageOptions](../interfaces/_index_d_._plugin_.messageoptions.md), ...`items`: T[]): [Thenable](../interfaces/_index_d_.thenable.md)\<T \| undefined>

*Defined in [index.d.ts:8461](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8461)*

Show a warning message.

**`see`** [showInformationMessage](#window.showInformationMessage)

#### Type parameters:

Name | Type |
------ | ------ |
`T` | [MessageItem](../interfaces/_index_d_._plugin_.messageitem.md) |

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`message` | string | The message to show. |
`options` | [MessageOptions](../interfaces/_index_d_._plugin_.messageoptions.md) | Configures the behaviour of the message. |
`...items` | T[] | A set of items that will be rendered as actions in the message. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<T \| undefined>

A thenable that resolves to the selected item or `undefined` when being dismissed.

___

### showWorkspaceFolderPick

▸ **showWorkspaceFolderPick**(`options?`: [WorkspaceFolderPickOptions](../interfaces/_index_d_._plugin_.workspacefolderpickoptions.md)): [Thenable](../interfaces/_index_d_.thenable.md)\<[WorkspaceFolder](../interfaces/_index_d_._plugin_.workspacefolder.md) \| undefined>

*Defined in [index.d.ts:8556](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8556)*

Shows a selection list of [workspace folders](#workspace.workspaceFolders) to pick from.
Returns `undefined` if no folder is open.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`options?` | [WorkspaceFolderPickOptions](../interfaces/_index_d_._plugin_.workspacefolderpickoptions.md) | Configures the behavior of the workspace folder list. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<[WorkspaceFolder](../interfaces/_index_d_._plugin_.workspacefolder.md) \| undefined>

A promise that resolves to the workspace folder or `undefined`.

___

### withProgress

▸ **withProgress**\<R>(`options`: [ProgressOptions](../interfaces/_index_d_._plugin_.progressoptions.md), `task`: (progress: [Progress](../interfaces/_index_d_._plugin_.progress.md)\<{ increment?: number ; message?: string  }>, token: [CancellationToken](../interfaces/_index_d_._plugin_.cancellationtoken.md)) => [Thenable](../interfaces/_index_d_.thenable.md)\<R>): [Thenable](../interfaces/_index_d_.thenable.md)\<R>

*Defined in [index.d.ts:8812](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8812)*

Show progress in the editor. Progress is shown while running the given callback
and while the promise it returned isn't resolved nor rejected. The location at which
progress should show (and other details) is defined via the passed [`ProgressOptions`](#ProgressOptions).

#### Type parameters:

Name |
------ |
`R` |

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`options` | [ProgressOptions](../interfaces/_index_d_._plugin_.progressoptions.md) | - |
`task` | (progress: [Progress](../interfaces/_index_d_._plugin_.progress.md)\<{ increment?: number ; message?: string  }>, token: [CancellationToken](../interfaces/_index_d_._plugin_.cancellationtoken.md)) => [Thenable](../interfaces/_index_d_.thenable.md)\<R> | A callback returning a promise. Progress state can be reported with the provided [progress](#Progress)-object.  To report discrete progress, use `increment` to indicate how much work has been completed. Each call with a `increment` value will be summed up and reflected as overall progress until 100% is reached (a value of e.g. `10` accounts for `10%` of work done). Note that currently only `ProgressLocation.Notification` is capable of showing discrete progress.  To monitor if the operation has been cancelled by the user, use the provided [`CancellationToken`](#CancellationToken). Note that currently only `ProgressLocation.Notification` is supporting to show a cancel button to cancel the long running operation.  |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<R>

The thenable the task-callback returned.

___

### withScmProgress

▸ **withScmProgress**\<R>(`task`: (progress: [Progress](../interfaces/_index_d_._plugin_.progress.md)\<number>) => [Thenable](../interfaces/_index_d_.thenable.md)\<R>): [Thenable](../interfaces/_index_d_.thenable.md)\<R>

*Defined in [index.d.ts:8791](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8791)*

Show progress in the Source Control viewlet while running the given callback and while
its returned promise isn't resolve or rejected.

**`deprecated`** Use `withProgress` instead.

#### Type parameters:

Name |
------ |
`R` |

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`task` | (progress: [Progress](../interfaces/_index_d_._plugin_.progress.md)\<number>) => [Thenable](../interfaces/_index_d_.thenable.md)\<R> | A callback returning a promise. Progress increments can be reported with the provided [progress](#Progress)-object. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<R>

The thenable the task did return.
