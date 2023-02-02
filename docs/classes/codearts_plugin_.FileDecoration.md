[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FileDecoration

# Class: FileDecoration

["@codearts/plugin"](../modules/_codearts_plugin_.md).FileDecoration

A file decoration represents metadata that can be rendered with a file.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.FileDecoration.md#constructor)

### Properties

- [badge](codearts_plugin_.FileDecoration.md#badge)
- [color](codearts_plugin_.FileDecoration.md#color)
- [propagate](codearts_plugin_.FileDecoration.md#propagate)
- [tooltip](codearts_plugin_.FileDecoration.md#tooltip)

## Constructors

### constructor

• **new FileDecoration**(`badge?`, `tooltip?`, `color?`)

Creates a new decoration.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `badge?` | `string` | A letter that represents the decoration. |
| `tooltip?` | `string` | The tooltip of the decoration. |
| `color?` | [`ThemeColor`](codearts_plugin_.ThemeColor.md) | The color of the decoration. |

#### Defined in

[index.d.ts:6708](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6708)

## Properties

### badge

• `Optional` **badge**: `string`

A very short string that represents this decoration.

#### Defined in

[index.d.ts:6683](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6683)

___

### color

• `Optional` **color**: [`ThemeColor`](codearts_plugin_.ThemeColor.md)

The color of this decoration.

#### Defined in

[index.d.ts:6693](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6693)

___

### propagate

• `Optional` **propagate**: `boolean`

A flag expressing that this decoration should be
propagated to its parents.

#### Defined in

[index.d.ts:6699](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6699)

___

### tooltip

• `Optional` **tooltip**: `string`

A human-readable tooltip for this decoration.

#### Defined in

[index.d.ts:6688](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6688)
