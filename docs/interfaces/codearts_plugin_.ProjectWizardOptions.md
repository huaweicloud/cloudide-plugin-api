[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ProjectWizardOptions

# Interface: ProjectWizardOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).ProjectWizardOptions

Options of project wizard.

## Table of contents

### Properties

- [iconPath](codearts_plugin_.ProjectWizardOptions.md#iconpath)
- [retainContextWhenHidden](codearts_plugin_.ProjectWizardOptions.md#retaincontextwhenhidden)

## Properties

### iconPath

• `Optional` **iconPath**: [`Uri`](../classes/codearts_plugin_.Uri.md)

The icon path for project wizard, which will show with the label.

#### Defined in

[index.d.ts:9475](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L9475)

___

### retainContextWhenHidden

• `Optional` **retainContextWhenHidden**: `boolean`

Controls if the webview element itself (iframe) is kept around even when the view
is no longer visible.

Normally the webview's html context is created when the view becomes visible
and destroyed when it is hidden. Extensions that have complex state
or UI can set the `retainContextWhenHidden` to make the editor keep the webview
context around, even when the webview moves to a background tab. When a webview using
`retainContextWhenHidden` becomes hidden, its scripts and other dynamic content are suspended.
When the view becomes visible again, the context is automatically restored
in the exact same state it was in originally. You cannot send messages to a
hidden webview, even with `retainContextWhenHidden` enabled.

`retainContextWhenHidden` has a high memory overhead and should only be used if
your view's context cannot be quickly saved and restored.

#### Defined in

[index.d.ts:9493](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L9493)
