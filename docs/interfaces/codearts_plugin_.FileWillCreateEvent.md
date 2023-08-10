[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FileWillCreateEvent

# Interface: FileWillCreateEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).FileWillCreateEvent

An event that is fired when files are going to be created.

To make modifications to the workspace before the files are created,
call the [`waitUntil`](codearts_plugin_.FileWillCreateEvent.md#waituntil)-function with a
thenable that resolves to a [workspace edit](../classes/codearts_plugin_.WorkspaceEdit.md).

## Table of contents

### Properties

- [files](codearts_plugin_.FileWillCreateEvent.md#files)
- [token](codearts_plugin_.FileWillCreateEvent.md#token)

### Methods

- [waitUntil](codearts_plugin_.FileWillCreateEvent.md#waituntil)

## Properties

### files

• `Readonly` **files**: readonly [`Uri`](../classes/codearts_plugin_.Uri.md)[]

The files that are going to be created.

#### Defined in

[index.d.ts:12018](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12018)

___

### token

• `Readonly` **token**: [`CancellationToken`](codearts_plugin_.CancellationToken.md)

A cancellation token.

#### Defined in

[index.d.ts:12013](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12013)

## Methods

### waitUntil

▸ **waitUntil**(`thenable`): `void`

Allows to pause the event and to apply a [workspace edit](../classes/codearts_plugin_.WorkspaceEdit.md).

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
| `thenable` | [`Thenable`](Thenable.md)<[`WorkspaceEdit`](../classes/codearts_plugin_.WorkspaceEdit.md)\> | A thenable that delays saving. |

#### Returns

`void`

#### Defined in

[index.d.ts:12038](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12038)

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

[index.d.ts:12047](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12047)
