[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FileWillRenameEvent

# Interface: FileWillRenameEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).FileWillRenameEvent

An event that is fired when files are going to be renamed.

To make modifications to the workspace before the files are renamed,
call the [`waitUntil](codearts_plugin_.FileWillCreateEvent.md#waituntil)-function with a
thenable that resolves to a [workspace edit](../classes/codearts_plugin_.WorkspaceEdit.md).

## Table of contents

### Properties

- [files](codearts_plugin_.FileWillRenameEvent.md#files)
- [token](codearts_plugin_.FileWillRenameEvent.md#token)

### Methods

- [waitUntil](codearts_plugin_.FileWillRenameEvent.md#waituntil)

## Properties

### files

• `Readonly` **files**: readonly { `newUri`: [`Uri`](../classes/codearts_plugin_.Uri.md) ; `oldUri`: [`Uri`](../classes/codearts_plugin_.Uri.md)  }[]

The files that are going to be renamed.

#### Defined in

[index.d.ts:12109](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12109)

___

### token

• `Readonly` **token**: [`CancellationToken`](codearts_plugin_.CancellationToken.md)

A cancellation token.

#### Defined in

[index.d.ts:12104](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12104)

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

[index.d.ts:12129](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12129)

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

[index.d.ts:12138](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12138)
