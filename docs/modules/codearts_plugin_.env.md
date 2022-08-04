[@codearts/plugin](../README.md) / ["@codearts/plugin"](_codearts_plugin_.md) / env

# Namespace: env

["@codearts/plugin"](_codearts_plugin_.md).env

## Table of contents

### Variables

- [appHost](codearts_plugin_.env.md#apphost)
- [appName](codearts_plugin_.env.md#appname)
- [appRoot](codearts_plugin_.env.md#approot)
- [clipboard](codearts_plugin_.env.md#clipboard)
- [isNewAppInstall](codearts_plugin_.env.md#isnewappinstall)
- [isTelemetryEnabled](codearts_plugin_.env.md#istelemetryenabled)
- [language](codearts_plugin_.env.md#language)
- [machineId](codearts_plugin_.env.md#machineid)
- [remoteName](codearts_plugin_.env.md#remotename)
- [sessionId](codearts_plugin_.env.md#sessionid)
- [shell](codearts_plugin_.env.md#shell)
- [uiKind](codearts_plugin_.env.md#uikind)
- [uriScheme](codearts_plugin_.env.md#urischeme)

### Functions

- [asExternalUri](codearts_plugin_.env.md#asexternaluri)
- [onDidChangeTelemetryEnabled](codearts_plugin_.env.md#ondidchangetelemetryenabled)
- [openExternal](codearts_plugin_.env.md#openexternal)

## Variables

### appHost

• **appHost**: `string`

#### Defined in

[index.d.ts:9030](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9030)

___

### appName

• **appName**: `string`

#### Defined in

[index.d.ts:9014](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9014)

___

### appRoot

• **appRoot**: `string`

#### Defined in

[index.d.ts:9022](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9022)

___

### clipboard

• **clipboard**: [`Clipboard`](../interfaces/codearts_plugin_.Clipboard.md)

#### Defined in

[index.d.ts:9045](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9045)

___

### isNewAppInstall

• **isNewAppInstall**: `boolean`

#### Defined in

[index.d.ts:9062](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9062)

___

### isTelemetryEnabled

• **isTelemetryEnabled**: `boolean`

#### Defined in

[index.d.ts:9068](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9068)

___

### language

• **language**: `string`

#### Defined in

[index.d.ts:9040](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9040)

___

### machineId

• **machineId**: `string`

#### Defined in

[index.d.ts:9050](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9050)

___

### remoteName

• **remoteName**: `string` \| `undefined`

#### Defined in

[index.d.ts:9085](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9085)

___

### sessionId

• **sessionId**: `string`

#### Defined in

[index.d.ts:9056](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9056)

___

### shell

• **shell**: `string`

#### Defined in

[index.d.ts:9092](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9092)

___

### uiKind

• **uiKind**: [`UIKind`](../enums/codearts_plugin_.UIKind.md)

#### Defined in

[index.d.ts:9099](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9099)

___

### uriScheme

• **uriScheme**: `string`

#### Defined in

[index.d.ts:9035](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9035)

## Functions

### asExternalUri

▸ **asExternalUri**(`target`): [`Thenable`](../interfaces/Thenable.md)<[`Uri`](../classes/codearts_plugin_.Uri.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `target` | [`Uri`](../classes/codearts_plugin_.Uri.md) |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`Uri`](../classes/codearts_plugin_.Uri.md)\>

#### Defined in

[index.d.ts:9169](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9169)

___

### onDidChangeTelemetryEnabled

▸ `Const` **onDidChangeTelemetryEnabled**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: `boolean`) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9074](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9074)

___

### openExternal

▸ **openExternal**(`target`): [`Thenable`](../interfaces/Thenable.md)<`boolean`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`boolean`\>

#### Defined in

[index.d.ts:9114](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9114)
