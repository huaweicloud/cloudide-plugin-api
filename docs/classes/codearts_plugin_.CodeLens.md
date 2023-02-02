[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CodeLens

# Class: CodeLens

["@codearts/plugin"](../modules/_codearts_plugin_.md).CodeLens

A code lens represents a [Command](../interfaces/codearts_plugin_.Command.md) that should be shown along with
source text, like the number of references, a way to run tests, etc.

A code lens is _unresolved_ when no command is associated to it. For performance
reasons the creation of a code lens and resolving should be done to two stages.

**`See`**

 - [provideCodeLenses](../interfaces/codearts_plugin_.CodeLensProvider.md#providecodelenses)
 - [resolveCodeLens](../interfaces/codearts_plugin_.CodeLensProvider.md#resolvecodelens)

## Table of contents

### Constructors

- [constructor](codearts_plugin_.CodeLens.md#constructor)

### Properties

- [command](codearts_plugin_.CodeLens.md#command)
- [isResolved](codearts_plugin_.CodeLens.md#isresolved)
- [range](codearts_plugin_.CodeLens.md#range)

## Constructors

### constructor

• **new CodeLens**(`range`, `command?`)

Creates a new code lens object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](codearts_plugin_.Range.md) | The range to which this code lens applies. |
| `command?` | [`Command`](../interfaces/codearts_plugin_.Command.md) | The command associated to this code lens. |

#### Defined in

[index.d.ts:2603](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L2603)

## Properties

### command

• `Optional` **command**: [`Command`](../interfaces/codearts_plugin_.Command.md)

The command this code lens represents.

#### Defined in

[index.d.ts:2590](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L2590)

___

### isResolved

• `Readonly` **isResolved**: `boolean`

`true` when there is a command associated.

#### Defined in

[index.d.ts:2595](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L2595)

___

### range

• **range**: [`Range`](codearts_plugin_.Range.md)

The range in which this code lens is valid. Should only span a single line.

#### Defined in

[index.d.ts:2585](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L2585)
