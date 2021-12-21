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

*Defined in [index.d.ts:10716](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L10716)*

Checks if the given section has changed.
If scope is provided, checks if the section has changed for resources under the given scope.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`section` | string | Configuration name, supports _dotted_ names. |
`scope?` | [ConfigurationScope](../modules/_index_d_._plugin_.md#configurationscope) | A scope in which to check. |

**Returns:** boolean

`true` if the given section has changed.
