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

[index.d.ts:12007](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12007)

___

### token

• `Readonly` **token**: [`CancellationToken`](codearts_plugin_.CancellationToken.md)

A cancellation token.

#### Defined in

[index.d.ts:12002](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12002)

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

[index.d.ts:12027](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12027)

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

[index.d.ts:12036](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12036)
