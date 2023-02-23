[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / Plugin

# Interface: Plugin<T\>

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).Plugin

Represents an plugin.

To get an instance of an `Plugin` use [getPlugin](#plugins.getPlugin).

## Type parameters

| Name |
| :------ |
| `T` |

## Table of contents

### Properties

- [exports](cloudide_plugin_.Plugin.md#exports)
- [id](cloudide_plugin_.Plugin.md#id)
- [isActive](cloudide_plugin_.Plugin.md#isactive)
- [packageJSON](cloudide_plugin_.Plugin.md#packagejson)
- [pluginPath](cloudide_plugin_.Plugin.md#pluginpath)
- [pluginType](cloudide_plugin_.Plugin.md#plugintype)
- [pluginUri](cloudide_plugin_.Plugin.md#pluginuri)

### Methods

- [activate](cloudide_plugin_.Plugin.md#activate)

## Properties

### exports

• `Readonly` **exports**: `T`

The public API exported by this plug-in. It is an invalid action
to access this field before this plug-in has been activated.

#### Defined in

[index.d.ts:94](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L94)

___

### id

• `Readonly` **id**: `string`

The canonical plug-in identifier in the form of: `publisher.name`.

#### Defined in

[index.d.ts:63](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L63)

___

### isActive

• `Readonly` **isActive**: `boolean`

`true` if the plug-in has been activated.

#### Defined in

[index.d.ts:78](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L78)

___

### packageJSON

• `Readonly` **packageJSON**: `any`

The parsed contents of the plug-in's package.json.

#### Defined in

[index.d.ts:83](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L83)

___

### pluginPath

• `Readonly` **pluginPath**: `string`

The absolute file path of the directory containing this plug-in.

#### Defined in

[index.d.ts:68](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L68)

___

### pluginType

• `Readonly` **pluginType**: [`PluginType`](../modules/_cloudide_plugin_.md#plugintype)

#### Defined in

[index.d.ts:88](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L88)

___

### pluginUri

• `Readonly` **pluginUri**: [`Uri`](../classes/cloudide_plugin_.Uri.md)

The uri of the directory containing this plug-in.

#### Defined in

[index.d.ts:73](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L73)

## Methods

### activate

▸ **activate**(): `PromiseLike`<`T`\>

Activates this plug-in and returns its public API.

#### Returns

`PromiseLike`<`T`\>

A promise that will resolve when this plug-in has been activated.

#### Defined in

[index.d.ts:101](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L101)
