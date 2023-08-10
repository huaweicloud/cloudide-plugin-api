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

[index.d.ts:16931](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16931)

___

### isDefault

• `Optional` **isDefault**: `boolean`

#### Defined in

[index.d.ts:16932](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16932)

___

### label

• **label**: `string`

#### Defined in

[index.d.ts:16930](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16930)

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

[index.d.ts:16934](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16934)

___

### registeredRequestType

• `Optional` **registeredRequestType**: [`BuildRequestType`](../enums/codearts_plugin_.BuildRequestType.md)[]

#### Defined in

[index.d.ts:16933](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16933)
