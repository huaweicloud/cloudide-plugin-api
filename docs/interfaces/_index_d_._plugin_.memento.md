**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / Memento

# Interface: Memento

A memento represents a storage utility. It can store and retrieve
values.

## Hierarchy

* **Memento**

## Index

### Methods

* [get](_index_d_._plugin_.memento.md#get)
* [update](_index_d_._plugin_.memento.md#update)

## Methods

### get

▸ **get**\<T>(`key`: string): T \| undefined

*Defined in [index.d.ts:6070](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6070)*

Return a value.

#### Type parameters:

Name |
------ |
`T` |

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`key` | string | A string. |

**Returns:** T \| undefined

The stored value or `undefined`.

▸ **get**\<T>(`key`: string, `defaultValue`: T): T

*Defined in [index.d.ts:6080](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6080)*

Return a value.

#### Type parameters:

Name |
------ |
`T` |

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`key` | string | A string. |
`defaultValue` | T | A value that should be returned when there is no value (`undefined`) with the given key. |

**Returns:** T

The stored value or the defaultValue.

___

### update

▸ **update**(`key`: string, `value`: any): [Thenable](_index_d_.thenable.md)\<void>

*Defined in [index.d.ts:6088](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6088)*

Store a value. The value must be JSON-stringifyable.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`key` | string | A string. |
`value` | any | A value. MUST not contain cyclic references.  |

**Returns:** [Thenable](_index_d_.thenable.md)\<void>
