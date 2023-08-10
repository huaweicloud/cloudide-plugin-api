[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ProjectWizardOptions

# Interface: ProjectWizardOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).ProjectWizardOptions

Options of project wizard.

## Table of contents

### Properties

- [iconPath](codearts_plugin_.ProjectWizardOptions.md#iconpath)
- [index](codearts_plugin_.ProjectWizardOptions.md#index)
- [retainContextWhenHidden](codearts_plugin_.ProjectWizardOptions.md#retaincontextwhenhidden)

## Properties

### iconPath

• `Optional` **iconPath**: [`Uri`](../classes/codearts_plugin_.Uri.md)

The icon path for project wizard, which will show with the label.

#### Defined in

[index.d.ts:9580](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L9580)

___

### index

• `Optional` **index**: `number`

The index of project wizard,The value ranges from 0 to 2^32-2.
Sort from min to max.
If not defined, sort to the end.

#### Defined in

[index.d.ts:9605](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L9605)

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

[index.d.ts:9598](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L9598)
