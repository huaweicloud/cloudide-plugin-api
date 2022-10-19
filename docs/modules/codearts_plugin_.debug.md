[@codearts/plugin](../README.md) / ["@codearts/plugin"](_codearts_plugin_.md) / debug

# Namespace: debug

["@codearts/plugin"](_codearts_plugin_.md).debug

Namespace for debug functionality.

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

The currently active [debug console](../interfaces/codearts_plugin_.DebugConsole.md).
If no debug session is active, output sent to the debug console is not shown.

#### Defined in

[index.d.ts:14799](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L14799)

___

### activeDebugSession

• **activeDebugSession**: [`DebugSession`](../interfaces/codearts_plugin_.DebugSession.md) \| `undefined`

The currently active [debug session](../interfaces/codearts_plugin_.DebugSession.md) or `undefined`. The active debug session is the one
represented by the debug action floating window or the one currently shown in the drop down menu of the debug action floating window.
If no debug session is active, the value is `undefined`.

#### Defined in

[index.d.ts:14793](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L14793)

___

### breakpoints

• **breakpoints**: readonly [`Breakpoint`](../classes/codearts_plugin_.Breakpoint.md)[]

List of breakpoints.

#### Defined in

[index.d.ts:14804](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L14804)

## Functions

### addBreakpoints

▸ **addBreakpoints**(`breakpoints`): `void`

Add breakpoints.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `breakpoints` | readonly [`Breakpoint`](../classes/codearts_plugin_.Breakpoint.md)[] | The breakpoints to add. |

#### Returns

`void`

#### Defined in

[index.d.ts:14892](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L14892)

___

### asDebugSourceUri

▸ **asDebugSourceUri**(`source`, `session?`): [`Uri`](../classes/codearts_plugin_.Uri.md)

Converts a "Source" descriptor object received via the Debug Adapter Protocol into a Uri that can be used to load its contents.
If the source descriptor is based on a path, a file Uri is returned.
If the source descriptor uses a reference number, a specific debug Uri (scheme 'debug') is constructed that requires a corresponding ContentProvider and a running debug session

If the "Source" descriptor has insufficient information for creating the Uri, an error is thrown.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`DebugProtocolSource`](../interfaces/codearts_plugin_.DebugProtocolSource.md) | An object conforming to the [Source](https://microsoft.github.io/debug-adapter-protocol/specification#Types_Source) type defined in the Debug Adapter Protocol. |
| `session?` | [`DebugSession`](../interfaces/codearts_plugin_.DebugSession.md) | An optional debug session that will be used when the source descriptor uses a reference number to load the contents from an active debug session. |

#### Returns

[`Uri`](../classes/codearts_plugin_.Uri.md)

A uri that can be used to load the contents of the source.

#### Defined in

[index.d.ts:14911](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L14911)

___

### onDidChangeActiveDebugSession

▸ **onDidChangeActiveDebugSession**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: `undefined` \| [`DebugSession`](../interfaces/codearts_plugin_.DebugSession.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L1603)

___

### onDidChangeBreakpoints

▸ **onDidChangeBreakpoints**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`BreakpointsChangeEvent`](../interfaces/codearts_plugin_.BreakpointsChangeEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L1603)

___

### onDidReceiveDebugSessionCustomEvent

▸ **onDidReceiveDebugSessionCustomEvent**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`DebugSessionCustomEvent`](../interfaces/codearts_plugin_.DebugSessionCustomEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L1603)

___

### onDidStartDebugSession

▸ **onDidStartDebugSession**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`DebugSession`](../interfaces/codearts_plugin_.DebugSession.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L1603)

___

### onDidTerminateDebugSession

▸ **onDidTerminateDebugSession**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`DebugSession`](../interfaces/codearts_plugin_.DebugSession.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L1603)

___

### registerDebugAdapterDescriptorFactory

▸ **registerDebugAdapterDescriptorFactory**(`debugType`, `factory`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a [debug adapter descriptor factory](../interfaces/codearts_plugin_.DebugAdapterDescriptorFactory.md) for a specific debug type.
An extension is only allowed to register a DebugAdapterDescriptorFactory for the debug type(s) defined by the extension. Otherwise an error is thrown.
Registering more than one DebugAdapterDescriptorFactory for a debug type results in an error.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `debugType` | `string` | The debug type for which the factory is registered. |
| `factory` | [`DebugAdapterDescriptorFactory`](../interfaces/codearts_plugin_.DebugAdapterDescriptorFactory.md) | The [debug adapter descriptor factory](../interfaces/codearts_plugin_.DebugAdapterDescriptorFactory.md) to register. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this factory when being disposed.

#### Defined in

[index.d.ts:14858](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L14858)

___

### registerDebugAdapterTrackerFactory

▸ **registerDebugAdapterTrackerFactory**(`debugType`, `factory`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a debug adapter tracker factory for the given debug type.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `debugType` | `string` | The debug type for which the factory is registered or '*' for matching all debug types. |
| `factory` | [`DebugAdapterTrackerFactory`](../interfaces/codearts_plugin_.DebugAdapterTrackerFactory.md) | The [debug adapter tracker factory](../interfaces/codearts_plugin_.DebugAdapterTrackerFactory.md) to register. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this factory when being disposed.

#### Defined in

[index.d.ts:14867](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L14867)

___

### registerDebugConfigurationProvider

▸ **registerDebugConfigurationProvider**(`debugType`, `provider`, `triggerKind?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a [debug configuration provider](../interfaces/codearts_plugin_.DebugConfigurationProvider.md) for a specific debug type.
The optional [triggerKind](../enums/codearts_plugin_.DebugConfigurationProviderTriggerKind.md) can be used to specify when the `provideDebugConfigurations` method of the provider is triggered.
Currently two trigger kinds are possible: with the value `Initial` (or if no trigger kind argument is given) the `provideDebugConfigurations` method is used to provide the initial debug configurations to be copied into a newly created launch.json.
With the trigger kind `Dynamic` the `provideDebugConfigurations` method is used to dynamically determine debug configurations to be presented to the user (in addition to the static configurations from the launch.json).
Please note that the `triggerKind` argument only applies to the `provideDebugConfigurations` method: so the `resolveDebugConfiguration` methods are not affected at all.
Registering a single provider with resolve methods for different trigger kinds, results in the same resolve methods called multiple times.
More than one provider can be registered for the same type.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `debugType` | `string` | The debug type for which the provider is registered. |
| `provider` | [`DebugConfigurationProvider`](../interfaces/codearts_plugin_.DebugConfigurationProvider.md) | The [debug configuration provider](../interfaces/codearts_plugin_.DebugConfigurationProvider.md) to register. |
| `triggerKind?` | [`DebugConfigurationProviderTriggerKind`](../enums/codearts_plugin_.DebugConfigurationProviderTriggerKind.md) | The DebugConfigurationProviderTrigger trigger for which the 'provideDebugConfiguration' method of the provider is registered. If `triggerKind` is missing, the value `DebugConfigurationProviderTriggerKind.Initial` is assumed. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:14847](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L14847)

___

### removeBreakpoints

▸ **removeBreakpoints**(`breakpoints`): `void`

Remove breakpoints.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `breakpoints` | readonly [`Breakpoint`](../classes/codearts_plugin_.Breakpoint.md)[] | The breakpoints to remove. |

#### Returns

`void`

#### Defined in

[index.d.ts:14898](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L14898)

___

### startDebugging

▸ **startDebugging**(`folder`, `nameOrConfiguration`, `parentSessionOrOptions?`): [`Thenable`](../interfaces/Thenable.md)<`boolean`\>

Start debugging by using either a named launch or named compound configuration,
or by directly passing a [DebugConfiguration](../interfaces/codearts_plugin_.DebugConfiguration.md).
The named configurations are looked up in '.arts/launch.json' found in the given folder.
Before debugging starts, all unsaved files are saved and the launch configurations are brought up-to-date.
Folder specific variables used in the configuration (e.g. '${workspaceFolder}') are resolved against the given folder.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `folder` | `undefined` \| [`WorkspaceFolder`](../interfaces/codearts_plugin_.WorkspaceFolder.md) | The [workspace folder](../interfaces/codearts_plugin_.WorkspaceFolder.md) for looking up named configurations and resolving variables or `undefined` for a non-folder setup. |
| `nameOrConfiguration` | `string` \| [`DebugConfiguration`](../interfaces/codearts_plugin_.DebugConfiguration.md) | Either the name of a debug or compound configuration or a [DebugConfiguration](../interfaces/codearts_plugin_.DebugConfiguration.md) object. |
| `parentSessionOrOptions?` | [`DebugSession`](../interfaces/codearts_plugin_.DebugSession.md) \| [`DebugSessionOptions`](../interfaces/codearts_plugin_.DebugSessionOptions.md) | Debug session options. When passed a parent [debug session](../interfaces/codearts_plugin_.DebugSession.md), assumes options with just this parent session. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`boolean`\>

A thenable that resolves when debugging could be successfully started.

#### Defined in

[index.d.ts:14880](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L14880)

___

### stopDebugging

▸ **stopDebugging**(`session?`): [`Thenable`](../interfaces/Thenable.md)<`void`\>

Stop the given debug session or stop all debug sessions if session is omitted.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `session?` | [`DebugSession`](../interfaces/codearts_plugin_.DebugSession.md) | The [debug session](../interfaces/codearts_plugin_.DebugSession.md) to stop; if omitted all sessions are stopped. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`void`\>

#### Defined in

[index.d.ts:14886](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L14886)
