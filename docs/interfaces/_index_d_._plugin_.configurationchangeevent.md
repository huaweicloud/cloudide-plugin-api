**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / ConfigurationChangeEvent

# Interface: ConfigurationChangeEvent

An event describing the change in Configuration

## Hierarchy

* **ConfigurationChangeEvent**

## Index

### Methods

* [affectsConfiguration](_index_d_._plugin_.configurationchangeevent.md#affectsconfiguration)

## Methods

### affectsConfiguration

▸ **affectsConfiguration**(`section`: string, `scope?`: [ConfigurationScope](../modules/_index_d_._plugin_.md#configurationscope)): boolean

*Defined in [index.d.ts:9372](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9372)*

Returns `true` if the given section is affected in the provided scope.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`section` | string | Configuration name, supports _dotted_ names. |
`scope?` | [ConfigurationScope](../modules/_index_d_._plugin_.md#configurationscope) | A scope in which to check. |

**Returns:** boolean

`true` if the given section is affected in the provided scope.
