[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SnippetString

# Class: SnippetString

["@codearts/plugin"](../modules/_codearts_plugin_.md).SnippetString

## Table of contents

### Constructors

- [constructor](codearts_plugin_.SnippetString.md#constructor)

### Properties

- [value](codearts_plugin_.SnippetString.md#value)

### Methods

- [appendChoice](codearts_plugin_.SnippetString.md#appendchoice)
- [appendPlaceholder](codearts_plugin_.SnippetString.md#appendplaceholder)
- [appendTabstop](codearts_plugin_.SnippetString.md#appendtabstop)
- [appendText](codearts_plugin_.SnippetString.md#appendtext)
- [appendVariable](codearts_plugin_.SnippetString.md#appendvariable)

## Constructors

### constructor

• **new SnippetString**(`value?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Defined in

[index.d.ts:3588](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L3588)

## Properties

### value

• **value**: `string`

#### Defined in

[index.d.ts:3586](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L3586)

## Methods

### appendChoice

▸ **appendChoice**(`values`, `number?`): [`SnippetString`](codearts_plugin_.SnippetString.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `values` | readonly `string`[] |  |
| `number?` | `number` |  |

#### Returns

[`SnippetString`](codearts_plugin_.SnippetString.md)

#### Defined in

[index.d.ts:3630](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L3630)

___

### appendPlaceholder

▸ **appendPlaceholder**(`value`, `number?`): [`SnippetString`](codearts_plugin_.SnippetString.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` \| (`snippet`: [`SnippetString`](codearts_plugin_.SnippetString.md)) => `any` |  |
| `number?` | `number` |  |

#### Returns

[`SnippetString`](codearts_plugin_.SnippetString.md)

#### Defined in

[index.d.ts:3619](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L3619)

___

### appendTabstop

▸ **appendTabstop**(`number?`): [`SnippetString`](codearts_plugin_.SnippetString.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `number?` | `number` |  |

#### Returns

[`SnippetString`](codearts_plugin_.SnippetString.md)

#### Defined in

[index.d.ts:3607](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L3607)

___

### appendText

▸ **appendText**(`string`): [`SnippetString`](codearts_plugin_.SnippetString.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `string` | `string` |  |

#### Returns

[`SnippetString`](codearts_plugin_.SnippetString.md)

#### Defined in

[index.d.ts:3597](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L3597)

___

### appendVariable

▸ **appendVariable**(`name`, `defaultValue`): [`SnippetString`](codearts_plugin_.SnippetString.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` |  |
| `defaultValue` | `string` \| (`snippet`: [`SnippetString`](codearts_plugin_.SnippetString.md)) => `any` |  |

#### Returns

[`SnippetString`](codearts_plugin_.SnippetString.md)

#### Defined in

[index.d.ts:3641](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L3641)
