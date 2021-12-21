**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / EnvironmentVariableCollection

# Interface: EnvironmentVariableCollection

A collection of mutations that an extension can apply to a process environment.

## Hierarchy

* **EnvironmentVariableCollection**

## Index

### Properties

* [persistent](_index_d_._plugin_.environmentvariablecollection.md#persistent)

### Methods

* [append](_index_d_._plugin_.environmentvariablecollection.md#append)
* [clear](_index_d_._plugin_.environmentvariablecollection.md#clear)
* [delete](_index_d_._plugin_.environmentvariablecollection.md#delete)
* [forEach](_index_d_._plugin_.environmentvariablecollection.md#foreach)
* [get](_index_d_._plugin_.environmentvariablecollection.md#get)
* [prepend](_index_d_._plugin_.environmentvariablecollection.md#prepend)
* [replace](_index_d_._plugin_.environmentvariablecollection.md#replace)

## Properties

### persistent

•  **persistent**: boolean

*Defined in [index.d.ts:9575](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9575)*

Whether the collection should be cached for the workspace and applied to the terminal
across window reloads. When true the collection will be active immediately such when the
window reloads. Additionally, this API will return the cached version if it exists. The
collection will be invalidated when the extension is uninstalled or when the collection
is cleared. Defaults to true.

## Methods

### append

▸ **append**(`variable`: string, `value`: string): void

*Defined in [index.d.ts:9597](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9597)*

Append a value to an environment variable.

Note that an extension can only make a single change to any one variable, so this will
overwrite any previous calls to replace, append or prepend.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`variable` | string | The variable to append to. |
`value` | string | The value to append to the variable.  |

**Returns:** void

___

### clear

▸ **clear**(): void

*Defined in [index.d.ts:9635](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9635)*

Clears all mutators from this collection.

**Returns:** void

___

### delete

▸ **delete**(`variable`: string): void

*Defined in [index.d.ts:9630](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9630)*

Deletes this collection's mutator for a variable.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`variable` | string | The variable to delete the mutator for.  |

**Returns:** void

___

### forEach

▸ **forEach**(`callback`: (variable: string, mutator: [EnvironmentVariableMutator](_index_d_._plugin_.environmentvariablemutator.md), collection: [EnvironmentVariableCollection](_index_d_._plugin_.environmentvariablecollection.md)) => any, `thisArg?`: any): void

*Defined in [index.d.ts:9623](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9623)*

Iterate over each mutator in this collection.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`callback` | (variable: string, mutator: [EnvironmentVariableMutator](_index_d_._plugin_.environmentvariablemutator.md), collection: [EnvironmentVariableCollection](_index_d_._plugin_.environmentvariablecollection.md)) => any | Function to execute for each entry. |
`thisArg?` | any | The `this` context used when invoking the handler function.  |

**Returns:** void

___

### get

▸ **get**(`variable`: string): [EnvironmentVariableMutator](_index_d_._plugin_.environmentvariablemutator.md) \| undefined

*Defined in [index.d.ts:9615](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9615)*

Gets the mutator that this collection applies to a variable, if any.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`variable` | string | The variable to get the mutator for.  |

**Returns:** [EnvironmentVariableMutator](_index_d_._plugin_.environmentvariablemutator.md) \| undefined

___

### prepend

▸ **prepend**(`variable`: string, `value`: string): void

*Defined in [index.d.ts:9608](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9608)*

Prepend a value to an environment variable.

Note that an extension can only make a single change to any one variable, so this will
overwrite any previous calls to replace, append or prepend.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`variable` | string | The variable to prepend. |
`value` | string | The value to prepend to the variable.  |

**Returns:** void

___

### replace

▸ **replace**(`variable`: string, `value`: string): void

*Defined in [index.d.ts:9586](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9586)*

Replace an environment variable with a value.

Note that an extension can only make a single change to any one variable, so this will
overwrite any previous calls to replace, append or prepend.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`variable` | string | The variable to replace. |
`value` | string | The value to replace the variable with.  |

**Returns:** void
