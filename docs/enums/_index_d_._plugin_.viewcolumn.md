**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / ViewColumn

# Enumeration: ViewColumn

Denotes a location of an editor in the window. Editors can be arranged in a grid
and each column represents one editor location in that grid by counting the editors
in order of their appearance.

## Index

### Enumeration members

* [Active](_index_d_._plugin_.viewcolumn.md#active)
* [Beside](_index_d_._plugin_.viewcolumn.md#beside)
* [Eight](_index_d_._plugin_.viewcolumn.md#eight)
* [Five](_index_d_._plugin_.viewcolumn.md#five)
* [Four](_index_d_._plugin_.viewcolumn.md#four)
* [Nine](_index_d_._plugin_.viewcolumn.md#nine)
* [One](_index_d_._plugin_.viewcolumn.md#one)
* [Seven](_index_d_._plugin_.viewcolumn.md#seven)
* [Six](_index_d_._plugin_.viewcolumn.md#six)
* [Three](_index_d_._plugin_.viewcolumn.md#three)
* [Two](_index_d_._plugin_.viewcolumn.md#two)

## Enumeration members

### Active

•  **Active**:  = -1

*Defined in [index.d.ts:5087](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5087)*

A *symbolic* editor column representing the currently active column. This value
can be used when opening editors, but the *resolved* [viewColumn](#TextEditor.viewColumn)-value
of editors will always be `One`, `Two`, `Three`,... or `undefined` but never `Active`.

___

### Beside

•  **Beside**:  = -2

*Defined in [index.d.ts:5093](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5093)*

A *symbolic* editor column representing the column to the side of the active one. This value
can be used when opening editors, but the *resolved* [viewColumn](#TextEditor.viewColumn)-value
of editors will always be `One`, `Two`, `Three`,... or `undefined` but never `Beside`.

___

### Eight

•  **Eight**:  = 8

*Defined in [index.d.ts:5125](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5125)*

The eighth editor column.

___

### Five

•  **Five**:  = 5

*Defined in [index.d.ts:5113](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5113)*

The fifth editor column.

___

### Four

•  **Four**:  = 4

*Defined in [index.d.ts:5109](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5109)*

The fourth editor column.

___

### Nine

•  **Nine**:  = 9

*Defined in [index.d.ts:5129](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5129)*

The ninth editor column.

___

### One

•  **One**:  = 1

*Defined in [index.d.ts:5097](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5097)*

The first editor column.

___

### Seven

•  **Seven**:  = 7

*Defined in [index.d.ts:5121](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5121)*

The seventh editor column.

___

### Six

•  **Six**:  = 6

*Defined in [index.d.ts:5117](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5117)*

The sixth editor column.

___

### Three

•  **Three**:  = 3

*Defined in [index.d.ts:5105](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5105)*

The third editor column.

___

### Two

•  **Two**:  = 2

*Defined in [index.d.ts:5101](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5101)*

The second editor column.
