**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / FileWillRenameEvent

# Interface: FileWillRenameEvent

An event that is fired when files are going to be renamed.

To make modifications to the workspace before the files are renamed,
call the [`waitUntil](#FileWillCreateEvent.waitUntil)-function with a
thenable that resolves to a [workspace edit](#WorkspaceEdit).

## Hierarchy

* **FileWillRenameEvent**

## Index

### Properties

* [files](_index_d_._plugin_.filewillrenameevent.md#files)

### Methods

* [waitUntil](_index_d_._plugin_.filewillrenameevent.md#waituntil)

## Properties

### files

• `Readonly` **files**: ReadonlyArray\<{ newUri: [Uri](../classes/_index_d_._plugin_.uri.md) ; oldUri: [Uri](../classes/_index_d_._plugin_.uri.md)  }>

*Defined in [index.d.ts:10214](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L10214)*

The files that are going to be renamed.

## Methods

### waitUntil

▸ **waitUntil**(`thenable`: [Thenable](_index_d_.thenable.md)\<[WorkspaceEdit](../classes/_index_d_._plugin_.workspaceedit.md)>): void

*Defined in [index.d.ts:10234](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L10234)*

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

*Defined in [index.d.ts:10243](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L10243)*

Allows to pause the event until the provided thenable resolves.

*Note:* This function can only be called during event dispatch.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`thenable` | [Thenable](_index_d_.thenable.md)\<any> | A thenable that delays saving.  |

**Returns:** void
