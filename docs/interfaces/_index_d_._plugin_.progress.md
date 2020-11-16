**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / Progress

# Interface: Progress\<T>

Defines a generalized way of reporting progress updates.

## Type parameters

Name |
------ |
`T` |

## Hierarchy

* **Progress**

## Index

### Methods

* [report](_index_d_._plugin_.progress.md#report)

## Methods

### report

▸ **report**(`value`: T): void

*Defined in [index.d.ts:5283](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5283)*

Report a progress update.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`value` | T | A progress item, like a message and/or an report on how much work finished  |

**Returns:** void
