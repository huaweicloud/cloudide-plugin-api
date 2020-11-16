**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CodeLens

# Class: CodeLens

A code lens represents a [command](#Command) that should be shown along with
source text, like the number of references, a way to run tests, etc.

A code lens is _unresolved_ when no command is associated to it. For performance
reasons the creation of a code lens and resolving should be done to two stages.

**`see`** [CodeLensProvider.provideCodeLenses](#CodeLensProvider.provideCodeLenses)

**`see`** [CodeLensProvider.resolveCodeLens](#CodeLensProvider.resolveCodeLens)

## Hierarchy

* **CodeLens**

## Index

### Constructors

* [constructor](_index_d_._plugin_.codelens.md#constructor)

### Properties

* [command](_index_d_._plugin_.codelens.md#command)
* [isResolved](_index_d_._plugin_.codelens.md#isresolved)
* [range](_index_d_._plugin_.codelens.md#range)

## Constructors

### constructor

\+ **new CodeLens**(`range`: [Range](_index_d_._plugin_.range.md), `command?`: [Command](../interfaces/_index_d_._plugin_.command.md)): [CodeLens](_index_d_._plugin_.codelens.md)

*Defined in [index.d.ts:2266](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2266)*

Creates a new code lens object.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`range` | [Range](_index_d_._plugin_.range.md) | The range to which this code lens applies. |
`command?` | [Command](../interfaces/_index_d_._plugin_.command.md) | The command associated to this code lens.  |

**Returns:** [CodeLens](_index_d_._plugin_.codelens.md)

## Properties

### command

• `Optional` **command**: [Command](../interfaces/_index_d_._plugin_.command.md)

*Defined in [index.d.ts:2261](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2261)*

The command this code lens represents.

___

### isResolved

• `Readonly` **isResolved**: boolean

*Defined in [index.d.ts:2266](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2266)*

`true` when there is a command associated.

___

### range

•  **range**: [Range](_index_d_._plugin_.range.md)

*Defined in [index.d.ts:2256](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2256)*

The range in which this code lens is valid. Should only span a single line.
