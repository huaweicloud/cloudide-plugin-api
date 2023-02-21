[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CodeLens

# Class: CodeLens

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CodeLens

A code lens represents a [command](#Command) that should be shown along with
source text, like the number of references, a way to run tests, etc.

A code lens is _unresolved_ when no command is associated to it. For performance
reasons the creation of a code lens and resolving should be done to two stages.

**`See`**

 - [CodeLensProvider.provideCodeLenses](#CodeLensProvider.provideCodeLenses)
 - [CodeLensProvider.resolveCodeLens](#CodeLensProvider.resolveCodeLens)

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.CodeLens.md#constructor)

### Properties

- [command](cloudide_plugin_.CodeLens.md#command)
- [isResolved](cloudide_plugin_.CodeLens.md#isresolved)
- [range](cloudide_plugin_.CodeLens.md#range)

## Constructors

### constructor

• **new CodeLens**(`range`, `command?`)

Creates a new code lens object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](cloudide_plugin_.Range.md) | The range to which this code lens applies. |
| `command?` | [`Command`](../interfaces/cloudide_plugin_.Command.md) | The command associated to this code lens. |

#### Defined in

[index.d.ts:8043](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8043)

## Properties

### command

• `Optional` **command**: [`Command`](../interfaces/cloudide_plugin_.Command.md)

The command this code lens represents.

#### Defined in

[index.d.ts:8030](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8030)

___

### isResolved

• `Readonly` **isResolved**: `boolean`

`true` when there is a command associated.

#### Defined in

[index.d.ts:8035](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8035)

___

### range

• **range**: [`Range`](cloudide_plugin_.Range.md)

The range in which this code lens is valid. Should only span a single line.

#### Defined in

[index.d.ts:8025](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8025)
