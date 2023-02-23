[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / EnvironmentVariableCollection

# Interface: EnvironmentVariableCollection

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).EnvironmentVariableCollection

A collection of mutations that an extension can apply to a process environment.

## Table of contents

### Properties

- [persistent](cloudide_plugin_.EnvironmentVariableCollection.md#persistent)

### Methods

- [append](cloudide_plugin_.EnvironmentVariableCollection.md#append)
- [clear](cloudide_plugin_.EnvironmentVariableCollection.md#clear)
- [delete](cloudide_plugin_.EnvironmentVariableCollection.md#delete)
- [forEach](cloudide_plugin_.EnvironmentVariableCollection.md#foreach)
- [get](cloudide_plugin_.EnvironmentVariableCollection.md#get)
- [prepend](cloudide_plugin_.EnvironmentVariableCollection.md#prepend)
- [replace](cloudide_plugin_.EnvironmentVariableCollection.md#replace)

## Properties

### persistent

• **persistent**: `boolean`

Whether the collection should be cached for the workspace and applied to the terminal
across window reloads. When true the collection will be active immediately such when the
window reloads. Additionally, this API will return the cached version if it exists. The
collection will be invalidated when the extension is uninstalled or when the collection
is cleared. Defaults to true.

#### Defined in

[index.d.ts:3058](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3058)

## Methods

### append

▸ **append**(`variable`, `value`): `void`

Append a value to an environment variable.

Note that an extension can only make a single change to any one variable, so this will
overwrite any previous calls to replace, append or prepend.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `variable` | `string` | The variable to append to. |
| `value` | `string` | The value to append to the variable. |

#### Returns

`void`

#### Defined in

[index.d.ts:3080](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3080)

___

### clear

▸ **clear**(): `void`

Clears all mutators from this collection.

#### Returns

`void`

#### Defined in

[index.d.ts:3118](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3118)

___

### delete

▸ **delete**(`variable`): `void`

Deletes this collection's mutator for a variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `variable` | `string` | The variable to delete the mutator for. |

#### Returns

`void`

#### Defined in

[index.d.ts:3113](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3113)

___

### forEach

▸ **forEach**(`callback`, `thisArg?`): `void`

Iterate over each mutator in this collection.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`variable`: `string`, `mutator`: [`EnvironmentVariableMutator`](cloudide_plugin_.EnvironmentVariableMutator.md), `collection`: [`EnvironmentVariableCollection`](cloudide_plugin_.EnvironmentVariableCollection.md)) => `any` | Function to execute for each entry. |
| `thisArg?` | `any` | The `this` context used when invoking the handler function. |

#### Returns

`void`

#### Defined in

[index.d.ts:3106](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3106)

___

### get

▸ **get**(`variable`): `undefined` \| [`EnvironmentVariableMutator`](cloudide_plugin_.EnvironmentVariableMutator.md)

Gets the mutator that this collection applies to a variable, if any.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `variable` | `string` | The variable to get the mutator for. |

#### Returns

`undefined` \| [`EnvironmentVariableMutator`](cloudide_plugin_.EnvironmentVariableMutator.md)

#### Defined in

[index.d.ts:3098](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3098)

___

### prepend

▸ **prepend**(`variable`, `value`): `void`

Prepend a value to an environment variable.

Note that an extension can only make a single change to any one variable, so this will
overwrite any previous calls to replace, append or prepend.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `variable` | `string` | The variable to prepend. |
| `value` | `string` | The value to prepend to the variable. |

#### Returns

`void`

#### Defined in

[index.d.ts:3091](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3091)

___

### replace

▸ **replace**(`variable`, `value`): `void`

Replace an environment variable with a value.

Note that an extension can only make a single change to any one variable, so this will
overwrite any previous calls to replace, append or prepend.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `variable` | `string` | The variable to replace. |
| `value` | `string` | The value to replace the variable with. |

#### Returns

`void`

#### Defined in

[index.d.ts:3069](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3069)
