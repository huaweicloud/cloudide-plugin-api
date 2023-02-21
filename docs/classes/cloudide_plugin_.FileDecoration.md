[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / FileDecoration

# Class: FileDecoration

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).FileDecoration

A file decoration represents metadata that can be rendered with a file.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.FileDecoration.md#constructor)

### Properties

- [badge](cloudide_plugin_.FileDecoration.md#badge)
- [color](cloudide_plugin_.FileDecoration.md#color)
- [propagate](cloudide_plugin_.FileDecoration.md#propagate)
- [tooltip](cloudide_plugin_.FileDecoration.md#tooltip)

## Constructors

### constructor

• **new FileDecoration**(`badge?`, `tooltip?`, `color?`)

Creates a new decoration.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `badge?` | `string` | A letter that represents the decoration. |
| `tooltip?` | `string` | The tooltip of the decoration. |
| `color?` | [`ThemeColor`](cloudide_plugin_.ThemeColor.md) | The color of the decoration. |

#### Defined in

[index.d.ts:2982](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2982)

## Properties

### badge

• `Optional` **badge**: `string`

A very short string that represents this decoration.

#### Defined in

[index.d.ts:2957](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2957)

___

### color

• `Optional` **color**: [`ThemeColor`](cloudide_plugin_.ThemeColor.md)

The color of this decoration.

#### Defined in

[index.d.ts:2967](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2967)

___

### propagate

• `Optional` **propagate**: `boolean`

A flag expressing that this decoration should be
propagated to its parents.

#### Defined in

[index.d.ts:2973](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2973)

___

### tooltip

• `Optional` **tooltip**: `string`

A human-readable tooltip for this decoration.

#### Defined in

[index.d.ts:2962](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2962)
