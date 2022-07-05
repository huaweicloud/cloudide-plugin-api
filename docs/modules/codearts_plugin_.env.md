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

[index.d.ts:9012](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L9012)

___

### appName

• **appName**: `string`

#### Defined in

[index.d.ts:8996](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L8996)

___

### appRoot

• **appRoot**: `string`

#### Defined in

[index.d.ts:9004](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L9004)

___

### clipboard

• **clipboard**: [`Clipboard`](../interfaces/codearts_plugin_.Clipboard.md)

#### Defined in

[index.d.ts:9027](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L9027)

___

### isNewAppInstall

• **isNewAppInstall**: `boolean`

#### Defined in

[index.d.ts:9044](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L9044)

___

### isTelemetryEnabled

• **isTelemetryEnabled**: `boolean`

#### Defined in

[index.d.ts:9050](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L9050)

___

### language

• **language**: `string`

#### Defined in

[index.d.ts:9022](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L9022)

___

### machineId

• **machineId**: `string`

#### Defined in

[index.d.ts:9032](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L9032)

___

### remoteName

• **remoteName**: `string` \| `undefined`

#### Defined in

[index.d.ts:9067](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L9067)

___

### sessionId

• **sessionId**: `string`

#### Defined in

[index.d.ts:9038](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L9038)

___

### shell

• **shell**: `string`

#### Defined in

[index.d.ts:9074](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L9074)

___

### uiKind

• **uiKind**: [`UIKind`](../enums/codearts_plugin_.UIKind.md)

#### Defined in

[index.d.ts:9081](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L9081)

___

### uriScheme

• **uriScheme**: `string`

#### Defined in

[index.d.ts:9017](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L9017)

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

[index.d.ts:9151](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L9151)

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

[index.d.ts:9056](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L9056)

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

[index.d.ts:9096](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L9096)
