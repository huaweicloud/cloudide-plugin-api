[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / FileWillDeleteEvent

# Interface: FileWillDeleteEvent

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).FileWillDeleteEvent

An event that is fired when files are going to be deleted.

To make modifications to the workspace before the files are deleted,
call the [`waitUntil](#FileWillCreateEvent.waitUntil)-function with a
thenable that resolves to a [workspace edit](#WorkspaceEdit).

## Table of contents

### Properties

- [files](cloudide_plugin_.FileWillDeleteEvent.md#files)

### Methods

- [waitUntil](cloudide_plugin_.FileWillDeleteEvent.md#waituntil)

## Properties

### files

• `Readonly` **files**: readonly [`Uri`](../classes/cloudide_plugin_.Uri.md)[]

The files that are going to be deleted.

#### Defined in

[index.d.ts:1754](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1754)

## Methods

### waitUntil

▸ **waitUntil**(`thenable`): `void`

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

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `thenable` | [`Thenable`](Thenable.md)<[`WorkspaceEdit`](../classes/cloudide_plugin_.WorkspaceEdit.md)\> | A thenable that delays saving. |

#### Returns

`void`

#### Defined in

[index.d.ts:1774](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1774)

▸ **waitUntil**(`thenable`): `void`

Allows to pause the event until the provided thenable resolves.

*Note:* This function can only be called during event dispatch.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `thenable` | [`Thenable`](Thenable.md)<`any`\> | A thenable that delays saving. |

#### Returns

`void`

#### Defined in

[index.d.ts:1783](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1783)
