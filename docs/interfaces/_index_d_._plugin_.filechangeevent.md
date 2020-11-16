**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / FileChangeEvent

# Interface: FileChangeEvent

The event filesystem providers must use to signal a file change.

## Hierarchy

* **FileChangeEvent**

## Index

### Properties

* [type](_index_d_._plugin_.filechangeevent.md#type)
* [uri](_index_d_._plugin_.filechangeevent.md#uri)

## Properties

### type

• `Readonly` **type**: [FileChangeType](../enums/_index_d_._plugin_.filechangetype.md)

*Defined in [index.d.ts:6363](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6363)*

The type of change.

___

### uri

• `Readonly` **uri**: [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:6368](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6368)*

The uri of the file that has changed.
