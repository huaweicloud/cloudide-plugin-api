[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TestRunProfile

# Interface: TestRunProfile

["@codearts/plugin"](../modules/_codearts_plugin_.md).TestRunProfile

## Table of contents

### Properties

- [configureHandler](codearts_plugin_.TestRunProfile.md#configurehandler)
- [isDefault](codearts_plugin_.TestRunProfile.md#isdefault)
- [kind](codearts_plugin_.TestRunProfile.md#kind)
- [label](codearts_plugin_.TestRunProfile.md#label)
- [tag](codearts_plugin_.TestRunProfile.md#tag)

### Methods

- [dispose](codearts_plugin_.TestRunProfile.md#dispose)
- [runHandler](codearts_plugin_.TestRunProfile.md#runhandler)

## Properties

### configureHandler

• **configureHandler**: `undefined` \| () => `void`

#### Defined in

[index.d.ts:15363](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L15363)

___

### isDefault

• **isDefault**: `boolean`

#### Defined in

[index.d.ts:15349](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L15349)

___

### kind

• `Readonly` **kind**: [`TestRunProfileKind`](../enums/codearts_plugin_.TestRunProfileKind.md)

#### Defined in

[index.d.ts:15340](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L15340)

___

### label

• **label**: `string`

#### Defined in

[index.d.ts:15334](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L15334)

___

### tag

• **tag**: `undefined` \| [`TestTag`](../classes/codearts_plugin_.TestTag.md)

#### Defined in

[index.d.ts:15355](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L15355)

## Methods

### dispose

▸ **dispose**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:15382](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L15382)

___

### runHandler

▸ **runHandler**(`request`, `token`): `void` \| [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `request` | [`TestRunRequest`](../classes/codearts_plugin_.TestRunRequest.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | - |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:15377](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L15377)
