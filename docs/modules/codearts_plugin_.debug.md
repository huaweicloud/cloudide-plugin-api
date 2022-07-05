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

[index.d.ts:14541](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L14541)

___

### activeDebugSession

• **activeDebugSession**: [`DebugSession`](../interfaces/codearts_plugin_.DebugSession.md) \| `undefined`

#### Defined in

[index.d.ts:14535](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L14535)

___

### breakpoints

• **breakpoints**: readonly [`Breakpoint`](../classes/codearts_plugin_.Breakpoint.md)[]

#### Defined in

[index.d.ts:14546](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L14546)

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

[index.d.ts:14634](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L14634)

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

[index.d.ts:14653](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L14653)

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

[index.d.ts:14553](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L14553)

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

[index.d.ts:14573](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L14573)

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

[index.d.ts:14563](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L14563)

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

[index.d.ts:14558](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L14558)

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

[index.d.ts:14568](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L14568)

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

[index.d.ts:14600](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L14600)

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

[index.d.ts:14609](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L14609)

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

[index.d.ts:14589](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L14589)

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

[index.d.ts:14640](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L14640)

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

[index.d.ts:14622](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L14622)

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

[index.d.ts:14628](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L14628)
