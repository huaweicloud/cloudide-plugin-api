[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / BuildProfileOptions

# Interface: BuildProfileOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).BuildProfileOptions

## Table of contents

### Properties

- [buildHandler](codearts_plugin_.BuildProfileOptions.md#buildhandler)
- [isDefault](codearts_plugin_.BuildProfileOptions.md#isdefault)
- [label](codearts_plugin_.BuildProfileOptions.md#label)
- [onDidChangeBuildTaskStatus](codearts_plugin_.BuildProfileOptions.md#ondidchangebuildtaskstatus)
- [registeredRequestType](codearts_plugin_.BuildProfileOptions.md#registeredrequesttype)

## Properties

### buildHandler

• **buildHandler**: (`request`: [`BuildRequestType`](../enums/codearts_plugin_.BuildRequestType.md)) => `void` \| [`Thenable`](Thenable.md)<`boolean` \| `void`\>

#### Type declaration

▸ (`request`): `void` \| [`Thenable`](Thenable.md)<`boolean` \| `void`\>

##### Parameters

| Name | Type |
| :------ | :------ |
| `request` | [`BuildRequestType`](../enums/codearts_plugin_.BuildRequestType.md) |

##### Returns

`void` \| [`Thenable`](Thenable.md)<`boolean` \| `void`\>

#### Defined in

[index.d.ts:16822](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16822)

___

### isDefault

• `Optional` **isDefault**: `boolean`

#### Defined in

[index.d.ts:16823](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16823)

___

### label

• **label**: `string`

#### Defined in

[index.d.ts:16821](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16821)

___

### onDidChangeBuildTaskStatus

• `Optional` **onDidChangeBuildTaskStatus**: (`data`: { `buildStatus`: [`BuildStatusType`](../enums/codearts_plugin_.BuildStatusType.md) ; `code?`: `number` ; `message?`: `string`  }) => `void`

#### Type declaration

▸ (`data`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `data` | `Object` |
| `data.buildStatus` | [`BuildStatusType`](../enums/codearts_plugin_.BuildStatusType.md) |
| `data.code?` | `number` |
| `data.message?` | `string` |

##### Returns

`void`

#### Defined in

[index.d.ts:16825](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16825)

___

### registeredRequestType

• `Optional` **registeredRequestType**: [`BuildRequestType`](../enums/codearts_plugin_.BuildRequestType.md)[]

#### Defined in

[index.d.ts:16824](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16824)
