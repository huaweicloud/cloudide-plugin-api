[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](_cloudide_plugin_.md) / debug

# Namespace: debug

["@cloudide/plugin"](_cloudide_plugin_.md).debug

Namespace for debug functionality.

## Table of contents

### Variables

- [activeDebugConsole](cloudide_plugin_.debug.md#activedebugconsole)
- [activeDebugSession](cloudide_plugin_.debug.md#activedebugsession)
- [breakpoints](cloudide_plugin_.debug.md#breakpoints)

### Functions

- [addBreakpoints](cloudide_plugin_.debug.md#addbreakpoints)
- [onDidChangeActiveDebugSession](cloudide_plugin_.debug.md#ondidchangeactivedebugsession)
- [onDidChangeBreakpoints](cloudide_plugin_.debug.md#ondidchangebreakpoints)
- [onDidReceiveDebugSessionCustomEvent](cloudide_plugin_.debug.md#ondidreceivedebugsessioncustomevent)
- [onDidStartDebugSession](cloudide_plugin_.debug.md#ondidstartdebugsession)
- [onDidTerminateDebugSession](cloudide_plugin_.debug.md#ondidterminatedebugsession)
- [registerDebugAdapterDescriptorFactory](cloudide_plugin_.debug.md#registerdebugadapterdescriptorfactory)
- [registerDebugAdapterTrackerFactory](cloudide_plugin_.debug.md#registerdebugadaptertrackerfactory)
- [registerDebugConfigurationProvider](cloudide_plugin_.debug.md#registerdebugconfigurationprovider)
- [removeBreakpoints](cloudide_plugin_.debug.md#removebreakpoints)
- [startDebugging](cloudide_plugin_.debug.md#startdebugging)

## Variables

### activeDebugConsole

• **activeDebugConsole**: [`DebugConsole`](../interfaces/cloudide_plugin_.DebugConsole.md)

The currently active [debug console](#DebugConsole).

#### Defined in

[index.d.ts:10053](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10053)

___

### activeDebugSession

• **activeDebugSession**: [`DebugSession`](../interfaces/cloudide_plugin_.DebugSession.md) \| `undefined`

The currently active [debug session](#DebugSession) or `undefined`. The active debug session is the one
represented by the debug action floating window or the one currently shown in the drop down menu of the debug action floating window.
If no debug session is active, the value is `undefined`.

#### Defined in

[index.d.ts:10048](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10048)

___

### breakpoints

• **breakpoints**: [`Breakpoint`](../classes/cloudide_plugin_.Breakpoint.md)[]

List of breakpoints.

#### Defined in

[index.d.ts:10058](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10058)

## Functions

### addBreakpoints

▸ **addBreakpoints**(`breakpoints`): `void`

Add breakpoints.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `breakpoints` | [`Breakpoint`](../classes/cloudide_plugin_.Breakpoint.md)[] | The breakpoints to add. |

#### Returns

`void`

#### Defined in

[index.d.ts:10141](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10141)

___

### onDidChangeActiveDebugSession

▸ **onDidChangeActiveDebugSession**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: `undefined` \| [`DebugSession`](../interfaces/cloudide_plugin_.DebugSession.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidChangeBreakpoints

▸ **onDidChangeBreakpoints**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`BreakpointsChangeEvent`](../interfaces/cloudide_plugin_.BreakpointsChangeEvent.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidReceiveDebugSessionCustomEvent

▸ **onDidReceiveDebugSessionCustomEvent**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`DebugSessionCustomEvent`](../interfaces/cloudide_plugin_.DebugSessionCustomEvent.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidStartDebugSession

▸ **onDidStartDebugSession**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`DebugSession`](../interfaces/cloudide_plugin_.DebugSession.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidTerminateDebugSession

▸ **onDidTerminateDebugSession**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`DebugSession`](../interfaces/cloudide_plugin_.DebugSession.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### registerDebugAdapterDescriptorFactory

▸ **registerDebugAdapterDescriptorFactory**(`debugType`, `factory`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a [debug adapter descriptor factory](#DebugAdapterDescriptorFactory) for a specific debug type.
An extension is only allowed to register a DebugAdapterDescriptorFactory for the debug type(s) defined by the extension. Otherwise an error is thrown.
Registering more than one DebugAdapterDescriptorFactory for a debug type results in an error.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `debugType` | `string` | The debug type for which the factory is registered. |
| `factory` | [`DebugAdapterDescriptorFactory`](../interfaces/cloudide_plugin_.DebugAdapterDescriptorFactory.md) | The [debug adapter descriptor factory](#DebugAdapterDescriptorFactory) to register. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this factory when being disposed.

#### Defined in

[index.d.ts:10096](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10096)

___

### registerDebugAdapterTrackerFactory

▸ **registerDebugAdapterTrackerFactory**(`debugType`, `factory`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a debug adapter tracker factory for the given debug type.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `debugType` | `string` | The debug type for which the factory is registered or '*' for matching all debug types. |
| `factory` | [`DebugAdapterTrackerFactory`](../interfaces/cloudide_plugin_.DebugAdapterTrackerFactory.md) | The [debug adapter tracker factory](#DebugAdapterTrackerFactory) to register. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this factory when being disposed.

#### Defined in

[index.d.ts:10122](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10122)

___

### registerDebugConfigurationProvider

▸ **registerDebugConfigurationProvider**(`debugType`, `provider`, `triggerKind?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a [debug configuration provider](../interfaces/cloudide_plugin_.DebugConfigurationProvider.md) for a specific debug type.
The optional [triggerKind](../enums/cloudide_plugin_.DebugConfigurationProviderTriggerKind.md) can be used to specify when the `provideDebugConfigurations` method of the provider is triggered.
Currently there are two situations:
 (1) providing debug configurations to populate a newly created `launch.json`
 (2) providing dynamically generated configurations when the user asks for them through the UI (e.g. via the "Select and Start Debugging" command).
Please note that the `triggerKind` argument only applies to the `provideDebugConfigurations` method, the `resolveDebugConfiguration` methods are not affected at all.
Registering a single provider with resolve methods for different trigger kinds results in the same resolve methods being called multiple times.
More than one provider can be registered for the same type.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `debugType` | `string` | The debug type for which the provider is registered. |
| `provider` | [`DebugConfigurationProvider`](../interfaces/cloudide_plugin_.DebugConfigurationProvider.md) | The [debug configuration provider](../interfaces/cloudide_plugin_.DebugConfigurationProvider.md) to register. |
| `triggerKind?` | [`DebugConfigurationProviderTriggerKind`](../enums/cloudide_plugin_.DebugConfigurationProviderTriggerKind.md) | The DebugConfigurationProviderTrigger trigger for which the 'provideDebugConfiguration' method of the provider is registered. If `triggerKind` is missing, the value `DebugConfigurationProviderTriggerKind.Initial` is assumed. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [Disposable](../classes/cloudide_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:10113](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10113)

___

### removeBreakpoints

▸ **removeBreakpoints**(`breakpoints`): `void`

Remove breakpoints.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `breakpoints` | [`Breakpoint`](../classes/cloudide_plugin_.Breakpoint.md)[] | The breakpoints to remove. |

#### Returns

`void`

#### Defined in

[index.d.ts:10148](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10148)

___

### startDebugging

▸ **startDebugging**(`folder`, `nameOrConfiguration`, `options`): `PromiseLike`<`boolean`\>

Start debugging by using either a named launch or named compound configuration,
or by directly passing a [DebugConfiguration](#DebugConfiguration).
The named configurations are looked up in '.vscode/launch.json' found in the given folder.
Before debugging starts, all unsaved files are saved and the launch configurations are brought up-to-date.
Folder specific variables used in the configuration (e.g. '${workspaceFolder}') are resolved against the given folder.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `folder` | `undefined` \| [`WorkspaceFolder`](../interfaces/cloudide_plugin_.WorkspaceFolder.md) | The [workspace folder](#WorkspaceFolder) for looking up named configurations and resolving variables or `undefined` for a non-folder setup. |
| `nameOrConfiguration` | `string` \| [`DebugConfiguration`](../interfaces/cloudide_plugin_.DebugConfiguration.md) | Either the name of a debug or compound configuration or a [DebugConfiguration](#DebugConfiguration) object. |
| `options` | [`DebugSessionOptions`](../interfaces/cloudide_plugin_.DebugSessionOptions.md) | - |

#### Returns

`PromiseLike`<`boolean`\>

A thenable that resolves when debugging could be successfully started.

#### Defined in

[index.d.ts:10134](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10134)
