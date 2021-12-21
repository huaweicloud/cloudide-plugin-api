**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / AccessibilityInformation

# Interface: AccessibilityInformation

Accessibility information which controls screen reader behavior.

## Hierarchy

* **AccessibilityInformation**

## Index

### Properties

* [label](_index_d_._plugin_.accessibilityinformation.md#label)
* [role](_index_d_._plugin_.accessibilityinformation.md#role)

## Properties

### label

•  **label**: string

*Defined in [index.d.ts:5494](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5494)*

Label to be read out by a screen reader once the item has focus.

___

### role

• `Optional` **role**: string

*Defined in [index.d.ts:5502](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5502)*

Role of the widget which defines how a screen reader interacts with it.
The role should be set in special cases when for example a tree-like element behaves like a checkbox.
If role is not specified VS Code will pick the appropriate role automatically.
More about aria roles can be found here https://w3c.github.io/aria/#widget_roles
