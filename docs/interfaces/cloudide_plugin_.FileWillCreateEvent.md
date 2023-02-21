[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / FileWillCreateEvent

# Interface: FileWillCreateEvent

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).FileWillCreateEvent

An event that is fired when files are going to be created.

To make modifications to the workspace before the files are created,
call the [`waitUntil](#FileWillCreateEvent.waitUntil)-function with a
thenable that resolves to a [workspace edit](#WorkspaceEdit).

## Table of contents

### Properties

- [files](cloudide_plugin_.FileWillCreateEvent.md#files)

### Methods

- [waitUntil](cloudide_plugin_.FileWillCreateEvent.md#waituntil)

## Properties

### files

• `Readonly` **files**: readonly [`Uri`](../classes/cloudide_plugin_.Uri.md)[]

The files that are going to be created.

#### Defined in

[index.d.ts:1699](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1699)

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

[index.d.ts:1719](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1719)

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

[index.d.ts:1728](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1728)
