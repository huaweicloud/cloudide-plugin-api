[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ExtensionContext

# Interface: ExtensionContext

["@codearts/plugin"](../modules/_codearts_plugin_.md).ExtensionContext

## Table of contents

### Properties

- [environmentVariableCollection](codearts_plugin_.ExtensionContext.md#environmentvariablecollection)
- [extension](codearts_plugin_.ExtensionContext.md#extension)
- [extensionMode](codearts_plugin_.ExtensionContext.md#extensionmode)
- [extensionPath](codearts_plugin_.ExtensionContext.md#extensionpath)
- [extensionUri](codearts_plugin_.ExtensionContext.md#extensionuri)
- [globalState](codearts_plugin_.ExtensionContext.md#globalstate)
- [globalStoragePath](codearts_plugin_.ExtensionContext.md#globalstoragepath)
- [globalStorageUri](codearts_plugin_.ExtensionContext.md#globalstorageuri)
- [logPath](codearts_plugin_.ExtensionContext.md#logpath)
- [logUri](codearts_plugin_.ExtensionContext.md#loguri)
- [secrets](codearts_plugin_.ExtensionContext.md#secrets)
- [storagePath](codearts_plugin_.ExtensionContext.md#storagepath)
- [storageUri](codearts_plugin_.ExtensionContext.md#storageuri)
- [subscriptions](codearts_plugin_.ExtensionContext.md#subscriptions)
- [workspaceState](codearts_plugin_.ExtensionContext.md#workspacestate)

### Methods

- [asAbsolutePath](codearts_plugin_.ExtensionContext.md#asabsolutepath)

## Properties

### environmentVariableCollection

• `Readonly` **environmentVariableCollection**: [`EnvironmentVariableCollection`](codearts_plugin_.EnvironmentVariableCollection.md)

#### Defined in

[index.d.ts:6878](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6878)

___

### extension

• `Readonly` **extension**: [`Extension`](codearts_plugin_.Extension.md)<`any`\>

#### Defined in

[index.d.ts:6969](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6969)

___

### extensionMode

• `Readonly` **extensionMode**: [`ExtensionMode`](../enums/codearts_plugin_.ExtensionMode.md)

#### Defined in

[index.d.ts:6964](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6964)

___

### extensionPath

• `Readonly` **extensionPath**: `string`

#### Defined in

[index.d.ts:6872](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6872)

___

### extensionUri

• `Readonly` **extensionUri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

#### Defined in

[index.d.ts:6866](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6866)

___

### globalState

• `Readonly` **globalState**: [`Memento`](codearts_plugin_.Memento.md) & { `setKeysForSync`: (`keys`: readonly `string`[]) => `void`  }

#### Defined in

[index.d.ts:6840](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6840)

___

### globalStoragePath

• `Readonly` **globalStoragePath**: `string`

#### Defined in

[index.d.ts:6938](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6938)

___

### globalStorageUri

• `Readonly` **globalStorageUri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

#### Defined in

[index.d.ts:6927](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6927)

___

### logPath

• `Readonly` **logPath**: `string`

#### Defined in

[index.d.ts:6957](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6957)

___

### logUri

• `Readonly` **logUri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

#### Defined in

[index.d.ts:6948](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6948)

___

### secrets

• `Readonly` **secrets**: [`SecretStorage`](codearts_plugin_.SecretStorage.md)

#### Defined in

[index.d.ts:6861](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6861)

___

### storagePath

• `Readonly` **storagePath**: `undefined` \| `string`

#### Defined in

[index.d.ts:6915](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6915)

___

### storageUri

• `Readonly` **storageUri**: `undefined` \| [`Uri`](../classes/codearts_plugin_.Uri.md)

#### Defined in

[index.d.ts:6903](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6903)

___

### subscriptions

• `Readonly` **subscriptions**: { `dispose`: () => `any`  }[]

#### Defined in

[index.d.ts:6828](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6828)

___

### workspaceState

• `Readonly` **workspaceState**: [`Memento`](codearts_plugin_.Memento.md)

#### Defined in

[index.d.ts:6834](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6834)

## Methods

### asAbsolutePath

▸ **asAbsolutePath**(`relativePath`): `string`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `relativePath` | `string` |  |

#### Returns

`string`

#### Defined in

[index.d.ts:6889](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6889)
