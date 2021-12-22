**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / [window](../modules/_index_d_._plugin_.window.md) / CustomizableDialogEvent

# Interface: CustomizableDialogEvent

Represents event of customizable,
used as the `onclose` callback parameter in `CustomizableDialogOptions`.

## Hierarchy

* [Event](_index_d_._plugin_.event.md)\<any>

  ↳ **CustomizableDialogEvent**

## Callable

▸ (`listener`: (e: any) => any, `thisArgs?`: any, `disposables?`: [Disposable](../classes/_index_d_._plugin_.disposable.md)[]): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:1628](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1628)*

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`listener` | (e: any) => any | The listener function will be called when the event happens. |
`thisArgs?` | any | The `this`-argument which will be used when calling the event listener. |
`disposables?` | [Disposable](../classes/_index_d_._plugin_.disposable.md)[] | An array to which a [disposable](#Disposable) will be added. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A disposable which unsubscribes the event listener.

## Index

### Properties

* [dialogData](_index_d_._plugin_.window.customizabledialogevent.md#dialogdata)
* [targetElement](_index_d_._plugin_.window.customizabledialogevent.md#targetelement)

## Properties

### dialogData

• `Optional` **dialogData**: string

*Defined in [index.d.ts:8702](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8702)*

You can get cloudideDialogApis by 'acquireCloudideDialogApi'.
And if you want to emit data out, you can call method 'acquireCloudideDialogApi.bindDialogData(data)',
so that you can get this data when the dialog closed.

___

### targetElement

• `Optional` **targetElement**: [DialogControlElement](_index_d_._plugin_.window.dialogcontrolelement.md)

*Defined in [index.d.ts:8696](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L8696)*

The target you clicked when close the dialog.
