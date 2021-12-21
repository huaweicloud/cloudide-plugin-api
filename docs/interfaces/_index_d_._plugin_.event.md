**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / Event

# Interface: Event\<T>

Represents a typed event.

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

**`example`** 
item.onDidChange(function(event) { console.log("Event happened: " + event); });

## Type parameters

Name |
------ |
`T` |

## Hierarchy

* **Event**

  ↳ [CustomizableDialogEvent](_index_d_._plugin_.window.customizabledialogevent.md)

## Callable

▸ (`listener`: (e: T) => any, `thisArgs?`: any, `disposables?`: [Disposable](../classes/_index_d_._plugin_.disposable.md)[]): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:1625](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1625)*

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`listener` | (e: T) => any | The listener function will be called when the event happens. |
`thisArgs?` | any | The `this`-argument which will be used when calling the event listener. |
`disposables?` | [Disposable](../classes/_index_d_._plugin_.disposable.md)[] | An array to which a [disposable](#Disposable) will be added. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A disposable which unsubscribes the event listener.
