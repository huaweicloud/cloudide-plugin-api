[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ConfigurationChangeEvent

# Interface: ConfigurationChangeEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).ConfigurationChangeEvent

An event describing the change in Configuration

## Table of contents

### Methods

- [affectsConfiguration](codearts_plugin_.ConfigurationChangeEvent.md#affectsconfiguration)

## Methods

### affectsConfiguration

▸ **affectsConfiguration**(`section`, `scope?`): `boolean`

Checks if the given section has changed.
If scope is provided, checks if the section has changed for resources under the given scope.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `section` | `string` | Configuration name, supports _dotted_ names. |
| `scope?` | [`ConfigurationScope`](../modules/_codearts_plugin_.md#configurationscope) | A scope in which to check. |

#### Returns

`boolean`

`true` if the given section has changed.

#### Defined in

[index.d.ts:13059](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L13059)
