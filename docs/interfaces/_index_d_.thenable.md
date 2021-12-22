**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / Thenable

# Interface: Thenable\<T>

Thenable is a common denominator between ES6 promises, Q, jquery.Deferred, WinJS.Promise,
and others. This API makes no assumption about what promise library is being used which
enables reusing existing code without migrating to a specific promise implementation. Still,
we recommend the use of native promises which are available in this editor.

## Type parameters

Name |
------ |
`T` |

## Hierarchy

* **Thenable**

## Index

### Methods

* [then](_index_d_.thenable.md#then)

## Methods

### then

▸ **then**\<TResult>(`onfulfilled?`: (value: T) => TResult \| [Thenable](_index_d_.thenable.md)\<TResult>, `onrejected?`: (reason: any) => TResult \| [Thenable](_index_d_.thenable.md)\<TResult>): [Thenable](_index_d_.thenable.md)\<TResult>

*Defined in [index.d.ts:12632](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L12632)*

Attaches callbacks for the resolution and/or rejection of the Promise.

#### Type parameters:

Name |
------ |
`TResult` |

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`onfulfilled?` | (value: T) => TResult \| [Thenable](_index_d_.thenable.md)\<TResult> | The callback to execute when the Promise is resolved. |
`onrejected?` | (reason: any) => TResult \| [Thenable](_index_d_.thenable.md)\<TResult> | The callback to execute when the Promise is rejected. |

**Returns:** [Thenable](_index_d_.thenable.md)\<TResult>

A Promise for the completion of which ever callback is executed.

▸ **then**\<TResult>(`onfulfilled?`: (value: T) => TResult \| [Thenable](_index_d_.thenable.md)\<TResult>, `onrejected?`: (reason: any) => void): [Thenable](_index_d_.thenable.md)\<TResult>

*Defined in [index.d.ts:12633](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L12633)*

#### Type parameters:

Name |
------ |
`TResult` |

#### Parameters:

Name | Type |
------ | ------ |
`onfulfilled?` | (value: T) => TResult \| [Thenable](_index_d_.thenable.md)\<TResult> |
`onrejected?` | (reason: any) => void |

**Returns:** [Thenable](_index_d_.thenable.md)\<TResult>
