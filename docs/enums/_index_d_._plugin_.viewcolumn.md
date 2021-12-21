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

*Defined in [index.d.ts:5381](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5381)*

A *symbolic* editor column representing the currently active column. This value
can be used when opening editors, but the *resolved* [viewColumn](#TextEditor.viewColumn)-value
of editors will always be `One`, `Two`, `Three`,... or `undefined` but never `Active`.

___

### Beside

•  **Beside**:  = -2

*Defined in [index.d.ts:5387](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5387)*

A *symbolic* editor column representing the column to the side of the active one. This value
can be used when opening editors, but the *resolved* [viewColumn](#TextEditor.viewColumn)-value
of editors will always be `One`, `Two`, `Three`,... or `undefined` but never `Beside`.

___

### Eight

•  **Eight**:  = 8

*Defined in [index.d.ts:5419](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5419)*

The eighth editor column.

___

### Five

•  **Five**:  = 5

*Defined in [index.d.ts:5407](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5407)*

The fifth editor column.

___

### Four

•  **Four**:  = 4

*Defined in [index.d.ts:5403](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5403)*

The fourth editor column.

___

### Nine

•  **Nine**:  = 9

*Defined in [index.d.ts:5423](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5423)*

The ninth editor column.

___

### One

•  **One**:  = 1

*Defined in [index.d.ts:5391](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5391)*

The first editor column.

___

### Seven

•  **Seven**:  = 7

*Defined in [index.d.ts:5415](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5415)*

The seventh editor column.

___

### Six

•  **Six**:  = 6

*Defined in [index.d.ts:5411](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5411)*

The sixth editor column.

___

### Three

•  **Three**:  = 3

*Defined in [index.d.ts:5399](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5399)*

The third editor column.

___

### Two

•  **Two**:  = 2

*Defined in [index.d.ts:5395](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5395)*

The second editor column.
