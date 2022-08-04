[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TestRun

# Interface: TestRun

["@codearts/plugin"](../modules/_codearts_plugin_.md).TestRun

## Table of contents

### Properties

- [isPersisted](codearts_plugin_.TestRun.md#ispersisted)
- [name](codearts_plugin_.TestRun.md#name)
- [token](codearts_plugin_.TestRun.md#token)

### Methods

- [appendOutput](codearts_plugin_.TestRun.md#appendoutput)
- [end](codearts_plugin_.TestRun.md#end)
- [enqueued](codearts_plugin_.TestRun.md#enqueued)
- [errored](codearts_plugin_.TestRun.md#errored)
- [failed](codearts_plugin_.TestRun.md#failed)
- [passed](codearts_plugin_.TestRun.md#passed)
- [skipped](codearts_plugin_.TestRun.md#skipped)
- [started](codearts_plugin_.TestRun.md#started)

## Properties

### isPersisted

• `Readonly` **isPersisted**: `boolean`

#### Defined in

[index.d.ts:15601](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15601)

___

### name

• `Readonly` **name**: `undefined` \| `string`

#### Defined in

[index.d.ts:15590](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15590)

___

### token

• `Readonly` **token**: [`CancellationToken`](codearts_plugin_.CancellationToken.md)

#### Defined in

[index.d.ts:15596](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15596)

## Methods

### appendOutput

▸ **appendOutput**(`output`, `location?`, `test?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `output` | `string` |  |
| `location?` | [`Location`](../classes/codearts_plugin_.Location.md) |  |
| `test?` | [`TestItem`](codearts_plugin_.TestItem.md) |  |

#### Returns

`void`

#### Defined in

[index.d.ts:15658](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15658)

___

### end

▸ **end**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:15664](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15664)

___

### enqueued

▸ **enqueued**(`test`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `test` | [`TestItem`](codearts_plugin_.TestItem.md) |  |

#### Returns

`void`

#### Defined in

[index.d.ts:15607](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15607)

___

### errored

▸ **errored**(`test`, `message`, `duration?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `test` | [`TestItem`](codearts_plugin_.TestItem.md) |  |
| `message` | [`TestMessage`](../classes/codearts_plugin_.TestMessage.md) \| readonly [`TestMessage`](../classes/codearts_plugin_.TestMessage.md)[] |  |
| `duration?` | `number` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:15639](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15639)

___

### failed

▸ **failed**(`test`, `message`, `duration?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `test` | [`TestItem`](codearts_plugin_.TestItem.md) |  |
| `message` | [`TestMessage`](../classes/codearts_plugin_.TestMessage.md) \| readonly [`TestMessage`](../classes/codearts_plugin_.TestMessage.md)[] |  |
| `duration?` | `number` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:15628](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15628)

___

### passed

▸ **passed**(`test`, `duration?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `test` | [`TestItem`](codearts_plugin_.TestItem.md) |  |
| `duration?` | `number` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:15646](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15646)

___

### skipped

▸ **skipped**(`test`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `test` | [`TestItem`](codearts_plugin_.TestItem.md) |  |

#### Returns

`void`

#### Defined in

[index.d.ts:15619](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15619)

___

### started

▸ **started**(`test`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `test` | [`TestItem`](codearts_plugin_.TestItem.md) |  |

#### Returns

`void`

#### Defined in

[index.d.ts:15613](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15613)
