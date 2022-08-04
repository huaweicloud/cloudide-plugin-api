[@codearts/plugin](../README.md) / ["@codearts/plugin"](_codearts_plugin_.md) / debug

# Namespace: debug

["@codearts/plugin"](_codearts_plugin_.md).debug

## Table of contents

### Variables

- [activeDebugConsole](codearts_plugin_.debug.md#activedebugconsole)
- [activeDebugSession](codearts_plugin_.debug.md#activedebugsession)
- [breakpoints](codearts_plugin_.debug.md#breakpoints)

### Functions

- [addBreakpoints](codearts_plugin_.debug.md#addbreakpoints)
- [asDebugSourceUri](codearts_plugin_.debug.md#asdebugsourceuri)
- [onDidChangeActiveDebugSession](codearts_plugin_.debug.md#ondidchangeactivedebugsession)
- [onDidChangeBreakpoints](codearts_plugin_.debug.md#ondidchangebreakpoints)
- [onDidReceiveDebugSessionCustomEvent](codearts_plugin_.debug.md#ondidreceivedebugsessioncustomevent)
- [onDidStartDebugSession](codearts_plugin_.debug.md#ondidstartdebugsession)
- [onDidTerminateDebugSession](codearts_plugin_.debug.md#ondidterminatedebugsession)
- [registerDebugAdapterDescriptorFactory](codearts_plugin_.debug.md#registerdebugadapterdescriptorfactory)
- [registerDebugAdapterTrackerFactory](codearts_plugin_.debug.md#registerdebugadaptertrackerfactory)
- [registerDebugConfigurationProvider](codearts_plugin_.debug.md#registerdebugconfigurationprovider)
- [removeBreakpoints](codearts_plugin_.debug.md#removebreakpoints)
- [startDebugging](codearts_plugin_.debug.md#startdebugging)
- [stopDebugging](codearts_plugin_.debug.md#stopdebugging)

## Variables

### activeDebugConsole

• **activeDebugConsole**: [`DebugConsole`](../interfaces/codearts_plugin_.DebugConsole.md)

#### Defined in

[index.d.ts:14571](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14571)

___

### activeDebugSession

• **activeDebugSession**: [`DebugSession`](../interfaces/codearts_plugin_.DebugSession.md) \| `undefined`

#### Defined in

[index.d.ts:14565](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14565)

___

### breakpoints

• **breakpoints**: readonly [`Breakpoint`](../classes/codearts_plugin_.Breakpoint.md)[]

#### Defined in

[index.d.ts:14576](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14576)

## Functions

### addBreakpoints

▸ **addBreakpoints**(`breakpoints`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `breakpoints` | readonly [`Breakpoint`](../classes/codearts_plugin_.Breakpoint.md)[] |  |

#### Returns

`void`

#### Defined in

[index.d.ts:14664](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14664)

___

### asDebugSourceUri

▸ **asDebugSourceUri**(`source`, `session?`): [`Uri`](../classes/codearts_plugin_.Uri.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`DebugProtocolSource`](../interfaces/codearts_plugin_.DebugProtocolSource.md) |  |
| `session?` | [`DebugSession`](../interfaces/codearts_plugin_.DebugSession.md) |  |

#### Returns

[`Uri`](../classes/codearts_plugin_.Uri.md)

#### Defined in

[index.d.ts:14683](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14683)

___

### onDidChangeActiveDebugSession

▸ `Const` **onDidChangeActiveDebugSession**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: `undefined` \| [`DebugSession`](../interfaces/codearts_plugin_.DebugSession.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:14583](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14583)

___

### onDidChangeBreakpoints

▸ `Const` **onDidChangeBreakpoints**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`BreakpointsChangeEvent`](../interfaces/codearts_plugin_.BreakpointsChangeEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:14603](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14603)

___

### onDidReceiveDebugSessionCustomEvent

▸ `Const` **onDidReceiveDebugSessionCustomEvent**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`DebugSessionCustomEvent`](../interfaces/codearts_plugin_.DebugSessionCustomEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:14593](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14593)

___

### onDidStartDebugSession

▸ `Const` **onDidStartDebugSession**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`DebugSession`](../interfaces/codearts_plugin_.DebugSession.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:14588](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14588)

___

### onDidTerminateDebugSession

▸ `Const` **onDidTerminateDebugSession**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`DebugSession`](../interfaces/codearts_plugin_.DebugSession.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:14598](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14598)

___

### registerDebugAdapterDescriptorFactory

▸ **registerDebugAdapterDescriptorFactory**(`debugType`, `factory`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `debugType` | `string` |  |
| `factory` | [`DebugAdapterDescriptorFactory`](../interfaces/codearts_plugin_.DebugAdapterDescriptorFactory.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:14630](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14630)

___

### registerDebugAdapterTrackerFactory

▸ **registerDebugAdapterTrackerFactory**(`debugType`, `factory`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `debugType` | `string` |  |
| `factory` | [`DebugAdapterTrackerFactory`](../interfaces/codearts_plugin_.DebugAdapterTrackerFactory.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:14639](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14639)

___

### registerDebugConfigurationProvider

▸ **registerDebugConfigurationProvider**(`debugType`, `provider`, `triggerKind?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `debugType` | `string` |  |
| `provider` | [`DebugConfigurationProvider`](../interfaces/codearts_plugin_.DebugConfigurationProvider.md) |  |
| `triggerKind?` | [`DebugConfigurationProviderTriggerKind`](../enums/codearts_plugin_.DebugConfigurationProviderTriggerKind.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:14619](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14619)

___

### removeBreakpoints

▸ **removeBreakpoints**(`breakpoints`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `breakpoints` | readonly [`Breakpoint`](../classes/codearts_plugin_.Breakpoint.md)[] |  |

#### Returns

`void`

#### Defined in

[index.d.ts:14670](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14670)

___

### startDebugging

▸ **startDebugging**(`folder`, `nameOrConfiguration`, `parentSessionOrOptions?`): [`Thenable`](../interfaces/Thenable.md)<`boolean`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `folder` | `undefined` \| [`WorkspaceFolder`](../interfaces/codearts_plugin_.WorkspaceFolder.md) |  |
| `nameOrConfiguration` | `string` \| [`DebugConfiguration`](../interfaces/codearts_plugin_.DebugConfiguration.md) |  |
| `parentSessionOrOptions?` | [`DebugSession`](../interfaces/codearts_plugin_.DebugSession.md) \| [`DebugSessionOptions`](../interfaces/codearts_plugin_.DebugSessionOptions.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`boolean`\>

#### Defined in

[index.d.ts:14652](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14652)

___

### stopDebugging

▸ **stopDebugging**(`session?`): [`Thenable`](../interfaces/Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `session?` | [`DebugSession`](../interfaces/codearts_plugin_.DebugSession.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`void`\>

#### Defined in

[index.d.ts:14658](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14658)
