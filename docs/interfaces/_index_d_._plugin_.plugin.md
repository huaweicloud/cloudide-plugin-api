**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / Plugin

# Interface: Plugin\<T>

Represents an plugin.

To get an instance of an `Plugin` use [getPlugin](#plugins.getPlugin).

## Type parameters

Name |
------ |
`T` |

## Hierarchy

* **Plugin**

## Index

### Properties

* [exports](_index_d_._plugin_.plugin.md#exports)
* [id](_index_d_._plugin_.plugin.md#id)
* [isActive](_index_d_._plugin_.plugin.md#isactive)
* [packageJSON](_index_d_._plugin_.plugin.md#packagejson)
* [pluginPath](_index_d_._plugin_.plugin.md#pluginpath)
* [pluginType](_index_d_._plugin_.plugin.md#plugintype)
* [pluginUri](_index_d_._plugin_.plugin.md#pluginuri)

### Methods

* [activate](_index_d_._plugin_.plugin.md#activate)

## Properties

### exports

• `Readonly` **exports**: T

*Defined in [index.d.ts:64](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L64)*

The public API exported by this plug-in. It is an invalid action
to access this field before this plug-in has been activated.

___

### id

• `Readonly` **id**: string

*Defined in [index.d.ts:33](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L33)*

The canonical plug-in identifier in the form of: `publisher.name`.

___

### isActive

• `Readonly` **isActive**: boolean

*Defined in [index.d.ts:48](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L48)*

`true` if the plug-in has been activated.

___

### packageJSON

• `Readonly` **packageJSON**: any

*Defined in [index.d.ts:53](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L53)*

The parsed contents of the plug-in's package.json.

___

### pluginPath

• `Readonly` **pluginPath**: string

*Defined in [index.d.ts:38](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L38)*

The absolute file path of the directory containing this plug-in.

___

### pluginType

• `Readonly` **pluginType**: [PluginType](../modules/_index_d_._plugin_.md#plugintype)

*Defined in [index.d.ts:58](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L58)*

___

### pluginUri

• `Readonly` **pluginUri**: [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:43](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L43)*

The uri of the directory containing this plug-in.

## Methods

### activate

▸ **activate**(): PromiseLike\<T>

*Defined in [index.d.ts:71](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L71)*

Activates this plug-in and returns its public API.

**Returns:** PromiseLike\<T>

A promise that will resolve when this plug-in has been activated.
