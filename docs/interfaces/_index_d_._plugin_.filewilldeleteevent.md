**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / FileWillDeleteEvent

# Interface: FileWillDeleteEvent

An event that is fired when files are going to be deleted.

To make modifications to the workspace before the files are deleted,
call the [`waitUntil](#FileWillCreateEvent.waitUntil)-function with a
thenable that resolves to a [workspace edit](#WorkspaceEdit).

## Hierarchy

* **FileWillDeleteEvent**

## Index

### Properties

* [files](_index_d_._plugin_.filewilldeleteevent.md#files)

### Methods

* [waitUntil](_index_d_._plugin_.filewilldeleteevent.md#waituntil)

## Properties

### files

• `Readonly` **files**: ReadonlyArray\<[Uri](../classes/_index_d_._plugin_.uri.md)>

*Defined in [index.d.ts:10179](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L10179)*

The files that are going to be deleted.

## Methods

### waitUntil

▸ **waitUntil**(`thenable`: [Thenable](_index_d_.thenable.md)\<[WorkspaceEdit](../classes/_index_d_._plugin_.workspaceedit.md)>): void

*Defined in [index.d.ts:10199](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L10199)*

Allows to pause the event and to apply a [workspace edit](#WorkspaceEdit).

*Note:* This function can only be called during event dispatch and not
in an asynchronous manner:

```ts
workspace.onWillCreateFiles(event => {
	// async, will *throw* an error
	setTimeout(() => event.waitUntil(promise));

	// sync, OK
	event.waitUntil(promise);
})
```

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`thenable` | [Thenable](_index_d_.thenable.md)\<[WorkspaceEdit](../classes/_index_d_._plugin_.workspaceedit.md)> | A thenable that delays saving.  |

**Returns:** void

▸ **waitUntil**(`thenable`: [Thenable](_index_d_.thenable.md)\<any>): void

*Defined in [index.d.ts:10208](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L10208)*

Allows to pause the event until the provided thenable resolves.

*Note:* This function can only be called during event dispatch.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`thenable` | [Thenable](_index_d_.thenable.md)\<any> | A thenable that delays saving.  |

**Returns:** void
