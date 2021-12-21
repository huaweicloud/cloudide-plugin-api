**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / QuickPickItem

# Interface: QuickPickItem

Represents an item that can be selected from
a list of items.

## Hierarchy

* **QuickPickItem**

## Index

### Properties

* [alwaysShow](_index_d_._plugin_.quickpickitem.md#alwaysshow)
* [description](_index_d_._plugin_.quickpickitem.md#description)
* [detail](_index_d_._plugin_.quickpickitem.md#detail)
* [label](_index_d_._plugin_.quickpickitem.md#label)
* [picked](_index_d_._plugin_.quickpickitem.md#picked)

## Properties

### alwaysShow

• `Optional` **alwaysShow**: boolean

*Defined in [index.d.ts:1779](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1779)*

Always show this item.

___

### description

• `Optional` **description**: string

*Defined in [index.d.ts:1760](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1760)*

A human-readable string which is rendered less prominent in the same line. Supports rendering of
[theme icons](#ThemeIcon) via the `$(<name>)`-syntax.

___

### detail

• `Optional` **detail**: string

*Defined in [index.d.ts:1766](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1766)*

A human-readable string which is rendered less prominent in a separate line. Supports rendering of
[theme icons](#ThemeIcon) via the `$(<name>)`-syntax.

___

### label

•  **label**: string

*Defined in [index.d.ts:1754](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1754)*

A human-readable string which is rendered prominent. Supports rendering of [theme icons](#ThemeIcon) via
the `$(<name>)`-syntax.

___

### picked

• `Optional` **picked**: boolean

*Defined in [index.d.ts:1774](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1774)*

Optional flag indicating if this item is picked initially.
(Only honored when the picker allows multiple selections.)

**`see`** [QuickPickOptions.canPickMany](#QuickPickOptions.canPickMany)
