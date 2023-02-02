[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / BuildProfileOptions

# Interface: BuildProfileOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).BuildProfileOptions

## Table of contents

### Properties

- [buildHandler](codearts_plugin_.BuildProfileOptions.md#buildhandler)
- [isDefault](codearts_plugin_.BuildProfileOptions.md#isdefault)
- [label](codearts_plugin_.BuildProfileOptions.md#label)
- [registeredRequestType](codearts_plugin_.BuildProfileOptions.md#registeredrequesttype)

## Properties

### buildHandler

• **buildHandler**: (`request`: [`BuildRequestType`](../enums/codearts_plugin_.BuildRequestType.md)) => `void` \| [`Thenable`](Thenable.md)<`void`\>

#### Type declaration

▸ (`request`): `void` \| [`Thenable`](Thenable.md)<`void`\>

##### Parameters

| Name | Type |
| :------ | :------ |
| `request` | [`BuildRequestType`](../enums/codearts_plugin_.BuildRequestType.md) |

##### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:16742](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16742)

___

### isDefault

• `Optional` **isDefault**: `boolean`

#### Defined in

[index.d.ts:16743](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16743)

___

### label

• **label**: `string`

#### Defined in

[index.d.ts:16741](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16741)

___

### registeredRequestType

• `Optional` **registeredRequestType**: [`BuildRequestType`](../enums/codearts_plugin_.BuildRequestType.md)[]

#### Defined in

[index.d.ts:16744](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16744)
