[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / AccessibilityInformation

# Interface: AccessibilityInformation

["@codearts/plugin"](../modules/_codearts_plugin_.md).AccessibilityInformation

Accessibility information which controls screen reader behavior.

## Table of contents

### Properties

- [label](codearts_plugin_.AccessibilityInformation.md#label)
- [role](codearts_plugin_.AccessibilityInformation.md#role)

## Properties

### label

• `Readonly` **label**: `string`

Label to be read out by a screen reader once the item has focus.

#### Defined in

[index.d.ts:6275](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6275)

___

### role

• `Optional` `Readonly` **role**: `string`

Role of the widget which defines how a screen reader interacts with it.
The role should be set in special cases when for example a tree-like element behaves like a checkbox.
If role is not specified the editor will pick the appropriate role automatically.
More about aria roles can be found here https://w3c.github.io/aria/#widget_roles

#### Defined in

[index.d.ts:6283](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6283)
