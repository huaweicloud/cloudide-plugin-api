**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / ProgressOptions

# Interface: ProgressOptions

Value-object describing where and how progress should show.

## Hierarchy

* **ProgressOptions**

## Index

### Properties

* [cancellable](_index_d_._plugin_.progressoptions.md#cancellable)
* [location](_index_d_._plugin_.progressoptions.md#location)
* [title](_index_d_._plugin_.progressoptions.md#title)

## Properties

### cancellable

• `Optional` **cancellable**: boolean

*Defined in [index.d.ts:9683](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9683)*

Controls if a cancel button should show to allow the user to
cancel the long running operation.  Note that currently only
`ProgressLocation.Notification` is supporting to show a cancel
button.

___

### location

•  **location**: [ProgressLocation](../enums/_index_d_._plugin_.progresslocation.md) \| { viewId: string  }

*Defined in [index.d.ts:9669](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9669)*

The location at which progress should show.

___

### title

• `Optional` **title**: string

*Defined in [index.d.ts:9675](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9675)*

A human-readable string which will be used to describe the
operation.
