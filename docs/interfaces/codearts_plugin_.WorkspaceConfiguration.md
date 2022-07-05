[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / WorkspaceConfiguration

# Interface: WorkspaceConfiguration

["@codearts/plugin"](../modules/_codearts_plugin_.md).WorkspaceConfiguration

## Indexable

▪ [key: `string`]: `any`

## Table of contents

### Methods

- [get](codearts_plugin_.WorkspaceConfiguration.md#get)
- [has](codearts_plugin_.WorkspaceConfiguration.md#has)
- [inspect](codearts_plugin_.WorkspaceConfiguration.md#inspect)
- [update](codearts_plugin_.WorkspaceConfiguration.md#update)

## Methods

### get

▸ **get**<`T`\>(`section`): `undefined` \| `T`

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `section` | `string` |  |

#### Returns

`undefined` \| `T`

#### Defined in

[index.d.ts:5689](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L5689)

▸ **get**<`T`\>(`section`, `defaultValue`): `T`

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `section` | `string` |  |
| `defaultValue` | `T` |  |

#### Returns

`T`

#### Defined in

[index.d.ts:5698](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L5698)

___

### has

▸ **has**(`section`): `boolean`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `section` | `string` |  |

#### Returns

`boolean`

#### Defined in

[index.d.ts:5706](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L5706)

___

### inspect

▸ **inspect**<`T`\>(`section`): `undefined` \| { `defaultLanguageValue?`: `T` ; `defaultValue?`: `T` ; `globalLanguageValue?`: `T` ; `globalValue?`: `T` ; `key`: `string` ; `languageIds?`: `string`[] ; `workspaceFolderLanguageValue?`: `T` ; `workspaceFolderValue?`: `T` ; `workspaceLanguageValue?`: `T` ; `workspaceValue?`: `T`  }

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `section` | `string` |  |

#### Returns

`undefined` \| { `defaultLanguageValue?`: `T` ; `defaultValue?`: `T` ; `globalLanguageValue?`: `T` ; `globalValue?`: `T` ; `key`: `string` ; `languageIds?`: `string`[] ; `workspaceFolderLanguageValue?`: `T` ; `workspaceFolderValue?`: `T` ; `workspaceLanguageValue?`: `T` ; `workspaceValue?`: `T`  }

#### Defined in

[index.d.ts:5722](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L5722)

___

### update

▸ **update**(`section`, `value`, `configurationTarget?`, `overrideInLanguage?`): [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `section` | `string` |  |
| `value` | `any` |  |
| `configurationTarget?` | ``null`` \| `boolean` \| [`ConfigurationTarget`](../enums/codearts_plugin_.ConfigurationTarget.md) |  |
| `overrideInLanguage?` | `boolean` |  |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:5768](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L5768)
