[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FileWillDeleteEvent

# Interface: FileWillDeleteEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).FileWillDeleteEvent

An event that is fired when files are going to be deleted.

To make modifications to the workspace before the files are deleted,
call the [`waitUntil](codearts_plugin_.FileWillCreateEvent.md#waituntil)-function with a
thenable that resolves to a [workspace edit](../classes/codearts_plugin_.WorkspaceEdit.md).

## Table of contents

### Properties

- [files](codearts_plugin_.FileWillDeleteEvent.md#files)
- [token](codearts_plugin_.FileWillDeleteEvent.md#token)

### Methods

- [waitUntil](codearts_plugin_.FileWillDeleteEvent.md#waituntil)

## Properties

### files

• `Readonly` **files**: readonly [`Uri`](../classes/codearts_plugin_.Uri.md)[]

The files that are going to be deleted.

#### Defined in

[index.d.ts:11947](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L11947)

___

### token

• `Readonly` **token**: [`CancellationToken`](codearts_plugin_.CancellationToken.md)

A cancellation token.

#### Defined in

[index.d.ts:11942](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L11942)

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

[index.d.ts:11967](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L11967)

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

[index.d.ts:11976](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L11976)
