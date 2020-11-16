**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / OutputChannel

# Interface: OutputChannel

An output channel is a container for readonly textual information.

To get an instance of an `OutputChannel` use
[createOutputChannel](#window.createOutputChannel).

## Hierarchy

* **OutputChannel**

## Index

### Properties

* [name](_index_d_._plugin_.outputchannel.md#name)

### Methods

* [append](_index_d_._plugin_.outputchannel.md#append)
* [appendLine](_index_d_._plugin_.outputchannel.md#appendline)
* [clear](_index_d_._plugin_.outputchannel.md#clear)
* [dispose](_index_d_._plugin_.outputchannel.md#dispose)
* [hide](_index_d_._plugin_.outputchannel.md#hide)
* [show](_index_d_._plugin_.outputchannel.md#show)

## Properties

### name

• `Readonly` **name**: string

*Defined in [index.d.ts:5143](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5143)*

The human-readable name of this output channel.

## Methods

### append

▸ **append**(`value`: string): void

*Defined in [index.d.ts:5150](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5150)*

Append the given value to the channel.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`value` | string | A string, falsy values will not be printed.  |

**Returns:** void

___

### appendLine

▸ **appendLine**(`value`: string): void

*Defined in [index.d.ts:5158](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5158)*

Append the given value and a line feed character
to the channel.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`value` | string | A string, falsy values will be printed.  |

**Returns:** void

___

### clear

▸ **clear**(): void

*Defined in [index.d.ts:5163](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5163)*

Removes all output from the channel.

**Returns:** void

___

### dispose

▸ **dispose**(): void

*Defined in [index.d.ts:5190](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5190)*

Dispose and free associated resources.

**Returns:** void

___

### hide

▸ **hide**(): void

*Defined in [index.d.ts:5185](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5185)*

Hide this channel from the UI.

**Returns:** void

___

### show

▸ **show**(`preserveFocus?`: boolean): void

*Defined in [index.d.ts:5170](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5170)*

Reveal this channel in the UI.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`preserveFocus?` | boolean | When `true` the channel will not take focus.  |

**Returns:** void

▸ **show**(`column?`: [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md), `preserveFocus?`: boolean): void

*Defined in [index.d.ts:5180](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5180)*

~~Reveal this channel in the UI.~~

**`deprecated`** Use the overload with just one parameter (`show(preserveFocus?: boolean): void`).

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`column?` | [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md) | This argument is **deprecated** and will be ignored. |
`preserveFocus?` | boolean | When `true` the channel will not take focus.  |

**Returns:** void
