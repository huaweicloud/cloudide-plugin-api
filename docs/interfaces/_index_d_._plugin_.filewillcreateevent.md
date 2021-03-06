**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / FileWillCreateEvent

# Interface: FileWillCreateEvent

An event that is fired when files are going to be created.

To make modifications to the workspace before the files are created,
call the [`waitUntil](#FileWillCreateEvent.waitUntil)-function with a
thenable that resolves to a [workspace edit](#WorkspaceEdit).

## Hierarchy

* **FileWillCreateEvent**

## Index

### Properties

* [files](_index_d_._plugin_.filewillcreateevent.md#files)

### Methods

* [waitUntil](_index_d_._plugin_.filewillcreateevent.md#waituntil)

## Properties

### files

• `Readonly` **files**: ReadonlyArray\<[Uri](../classes/_index_d_._plugin_.uri.md)>

*Defined in [index.d.ts:8734](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8734)*

The files that are going to be created.

## Methods

### waitUntil

▸ **waitUntil**(`thenable`: [Thenable](_index_d_.thenable.md)\<[WorkspaceEdit](../classes/_index_d_._plugin_.workspaceedit.md)>): void

*Defined in [index.d.ts:8754](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8754)*

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

*Defined in [index.d.ts:8763](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8763)*

Allows to pause the event until the provided thenable resolves.

*Note:* This function can only be called during event dispatch.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`thenable` | [Thenable](_index_d_.thenable.md)\<any> | A thenable that delays saving.  |

**Returns:** void
