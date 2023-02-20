**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / FileDecoration

# Class: FileDecoration

A file decoration represents metadata that can be rendered with a file.

## Hierarchy

* **FileDecoration**

## Index

### Constructors

* [constructor](_index_d_._plugin_.filedecoration.md#constructor)

### Properties

* [badge](_index_d_._plugin_.filedecoration.md#badge)
* [color](_index_d_._plugin_.filedecoration.md#color)
* [propagate](_index_d_._plugin_.filedecoration.md#propagate)
* [tooltip](_index_d_._plugin_.filedecoration.md#tooltip)

## Constructors

### constructor

\+ **new FileDecoration**(`badge?`: string, `tooltip?`: string, `color?`: [ThemeColor](_index_d_._plugin_.themecolor.md)): [FileDecoration](_index_d_._plugin_.filedecoration.md)

*Defined in [index.d.ts:5768](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L5768)*

Creates a new decoration.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`badge?` | string | A letter that represents the decoration. |
`tooltip?` | string | The tooltip of the decoration. |
`color?` | [ThemeColor](_index_d_._plugin_.themecolor.md) | The color of the decoration.  |

**Returns:** [FileDecoration](_index_d_._plugin_.filedecoration.md)

## Properties

### badge

• `Optional` **badge**: string

*Defined in [index.d.ts:5752](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L5752)*

A very short string that represents this decoration.

___

### color

• `Optional` **color**: [ThemeColor](_index_d_._plugin_.themecolor.md)

*Defined in [index.d.ts:5762](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L5762)*

The color of this decoration.

___

### propagate

• `Optional` **propagate**: boolean

*Defined in [index.d.ts:5768](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L5768)*

A flag expressing that this decoration should be
propagated to its parents.

___

### tooltip

• `Optional` **tooltip**: string

*Defined in [index.d.ts:5757](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L5757)*

A human-readable tooltip for this decoration.
