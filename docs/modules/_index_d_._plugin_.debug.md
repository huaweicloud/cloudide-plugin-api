**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](_index_d_.md) / ["plugin"](_index_d_._plugin_.md) / debug

# Namespace: debug

Namespace for debug functionality.

## Index

### Variables

* [activeDebugConsole](_index_d_._plugin_.debug.md#activedebugconsole)
* [activeDebugSession](_index_d_._plugin_.debug.md#activedebugsession)
* [breakpoints](_index_d_._plugin_.debug.md#breakpoints)
* [onDidChangeActiveDebugSession](_index_d_._plugin_.debug.md#ondidchangeactivedebugsession)
* [onDidChangeBreakpoints](_index_d_._plugin_.debug.md#ondidchangebreakpoints)
* [onDidReceiveDebugSessionCustomEvent](_index_d_._plugin_.debug.md#ondidreceivedebugsessioncustomevent)
* [onDidStartDebugSession](_index_d_._plugin_.debug.md#ondidstartdebugsession)
* [onDidTerminateDebugSession](_index_d_._plugin_.debug.md#ondidterminatedebugsession)

### Functions

* [addBreakpoints](_index_d_._plugin_.debug.md#addbreakpoints)
* [asDebugSourceUri](_index_d_._plugin_.debug.md#asdebugsourceuri)
* [registerDebugAdapterDescriptorFactory](_index_d_._plugin_.debug.md#registerdebugadapterdescriptorfactory)
* [registerDebugAdapterTrackerFactory](_index_d_._plugin_.debug.md#registerdebugadaptertrackerfactory)
* [registerDebugConfigurationProvider](_index_d_._plugin_.debug.md#registerdebugconfigurationprovider)
* [removeBreakpoints](_index_d_._plugin_.debug.md#removebreakpoints)
* [startDebugging](_index_d_._plugin_.debug.md#startdebugging)

## Variables

### activeDebugConsole

• `Let` **activeDebugConsole**: [DebugConsole](../interfaces/_index_d_._plugin_.debugconsole.md)

*Defined in [index.d.ts:10545](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10545)*

The currently active [debug console](#DebugConsole).
If no debug session is active, output sent to the debug console is not shown.

___

### activeDebugSession

• `Let` **activeDebugSession**: [DebugSession](../interfaces/_index_d_._plugin_.debugsession.md) \| undefined

*Defined in [index.d.ts:10539](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10539)*

The currently active [debug session](#DebugSession) or `undefined`. The active debug session is the one
represented by the debug action floating window or the one currently shown in the drop down menu of the debug action floating window.
If no debug session is active, the value is `undefined`.

___

### breakpoints

• `Let` **breakpoints**: [Breakpoint](../classes/_index_d_._plugin_.breakpoint.md)[]

*Defined in [index.d.ts:10550](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10550)*

List of breakpoints.

___

### onDidChangeActiveDebugSession

• `Const` **onDidChangeActiveDebugSession**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[DebugSession](../interfaces/_index_d_._plugin_.debugsession.md) \| undefined>

*Defined in [index.d.ts:10558](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10558)*

An [event](#Event) which fires when the [active debug session](#debug.activeDebugSession)
has changed. *Note* that the event also fires when the active debug session changes
to `undefined`.

___

### onDidChangeBreakpoints

• `Const` **onDidChangeBreakpoints**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[BreakpointsChangeEvent](../interfaces/_index_d_._plugin_.breakpointschangeevent.md)>

*Defined in [index.d.ts:10578](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10578)*

An [event](#Event) that is emitted when the set of breakpoints is added, removed, or changed.

___

### onDidReceiveDebugSessionCustomEvent

• `Const` **onDidReceiveDebugSessionCustomEvent**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[DebugSessionCustomEvent](../interfaces/_index_d_._plugin_.debugsessioncustomevent.md)>

*Defined in [index.d.ts:10568](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10568)*

An [event](#Event) which fires when a custom DAP event is received from the [debug session](#DebugSession).

___

### onDidStartDebugSession

• `Const` **onDidStartDebugSession**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[DebugSession](../interfaces/_index_d_._plugin_.debugsession.md)>

*Defined in [index.d.ts:10563](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10563)*

An [event](#Event) which fires when a new [debug session](#DebugSession) has been started.

___

### onDidTerminateDebugSession

• `Const` **onDidTerminateDebugSession**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[DebugSession](../interfaces/_index_d_._plugin_.debugsession.md)>

*Defined in [index.d.ts:10573](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10573)*

An [event](#Event) which fires when a [debug session](#DebugSession) has terminated.

## Functions

### addBreakpoints

▸ **addBreakpoints**(`breakpoints`: [Breakpoint](../classes/_index_d_._plugin_.breakpoint.md)[]): void

*Defined in [index.d.ts:10627](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10627)*

Add breakpoints.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`breakpoints` | [Breakpoint](../classes/_index_d_._plugin_.breakpoint.md)[] | The breakpoints to add.  |

**Returns:** void

___

### asDebugSourceUri

▸ **asDebugSourceUri**(`source`: [DebugProtocolSource](../interfaces/_index_d_._plugin_.debugprotocolsource.md), `session?`: [DebugSession](../interfaces/_index_d_._plugin_.debugsession.md)): [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:10646](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10646)*

Converts a "Source" descriptor object received via the Debug Adapter Protocol into a Uri that can be used to load its contents.
If the source descriptor is based on a path, a file Uri is returned.
If the source descriptor uses a reference number, a specific debug Uri (scheme 'debug') is constructed that requires a corresponding VS Code ContentProvider and a running debug session

If the "Source" descriptor has insufficient information for creating the Uri, an error is thrown.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`source` | [DebugProtocolSource](../interfaces/_index_d_._plugin_.debugprotocolsource.md) | An object conforming to the [Source](https://microsoft.github.io/debug-adapter-protocol/specification#Types_Source) type defined in the Debug Adapter Protocol. |
`session?` | [DebugSession](../interfaces/_index_d_._plugin_.debugsession.md) | An optional debug session that will be used when the source descriptor uses a reference number to load the contents from an active debug session. |

**Returns:** [Uri](../classes/_index_d_._plugin_.uri.md)

A uri that can be used to load the contents of the source.

___

### registerDebugAdapterDescriptorFactory

▸ **registerDebugAdapterDescriptorFactory**(`debugType`: string, `factory`: [DebugAdapterDescriptorFactory](../interfaces/_index_d_._plugin_.debugadapterdescriptorfactory.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:10599](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10599)*

Register a [debug adapter descriptor factory](#DebugAdapterDescriptorFactory) for a specific debug type.
An extension is only allowed to register a DebugAdapterDescriptorFactory for the debug type(s) defined by the extension. Otherwise an error is thrown.
Registering more than one DebugAdapterDescriptorFactory for a debug type results in an error.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`debugType` | string | The debug type for which the factory is registered. |
`factory` | [DebugAdapterDescriptorFactory](../interfaces/_index_d_._plugin_.debugadapterdescriptorfactory.md) | The [debug adapter descriptor factory](#DebugAdapterDescriptorFactory) to register. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this factory when being disposed.

___

### registerDebugAdapterTrackerFactory

▸ **registerDebugAdapterTrackerFactory**(`debugType`: string, `factory`: [DebugAdapterTrackerFactory](../interfaces/_index_d_._plugin_.debugadaptertrackerfactory.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:10608](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10608)*

Register a debug adapter tracker factory for the given debug type.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`debugType` | string | The debug type for which the factory is registered or '*' for matching all debug types. |
`factory` | [DebugAdapterTrackerFactory](../interfaces/_index_d_._plugin_.debugadaptertrackerfactory.md) | The [debug adapter tracker factory](#DebugAdapterTrackerFactory) to register. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this factory when being disposed.

___

### registerDebugConfigurationProvider

▸ **registerDebugConfigurationProvider**(`debugType`: string, `provider`: [DebugConfigurationProvider](../interfaces/_index_d_._plugin_.debugconfigurationprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:10588](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10588)*

Register a [debug configuration provider](#DebugConfigurationProvider) for a specific debug type.
More than one provider can be registered for the same type.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`debugType` | string | - |
`provider` | [DebugConfigurationProvider](../interfaces/_index_d_._plugin_.debugconfigurationprovider.md) | The [debug configuration provider](#DebugConfigurationProvider) to register. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### removeBreakpoints

▸ **removeBreakpoints**(`breakpoints`: [Breakpoint](../classes/_index_d_._plugin_.breakpoint.md)[]): void

*Defined in [index.d.ts:10633](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10633)*

Remove breakpoints.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`breakpoints` | [Breakpoint](../classes/_index_d_._plugin_.breakpoint.md)[] | The breakpoints to remove.  |

**Returns:** void

___

### startDebugging

▸ **startDebugging**(`folder`: [WorkspaceFolder](../interfaces/_index_d_._plugin_.workspacefolder.md) \| undefined, `nameOrConfiguration`: string \| [DebugConfiguration](../interfaces/_index_d_._plugin_.debugconfiguration.md), `parentSessionOrOptions?`: [DebugSession](../interfaces/_index_d_._plugin_.debugsession.md) \| [DebugSessionOptions](../interfaces/_index_d_._plugin_.debugsessionoptions.md)): [Thenable](../interfaces/_index_d_.thenable.md)\<boolean>

*Defined in [index.d.ts:10621](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10621)*

Start debugging by using either a named launch or named compound configuration,
or by directly passing a [DebugConfiguration](#DebugConfiguration).
The named configurations are looked up in '.vscode/launch.json' found in the given folder.
Before debugging starts, all unsaved files are saved and the launch configurations are brought up-to-date.
Folder specific variables used in the configuration (e.g. '${workspaceFolder}') are resolved against the given folder.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`folder` | [WorkspaceFolder](../interfaces/_index_d_._plugin_.workspacefolder.md) \| undefined | The [workspace folder](#WorkspaceFolder) for looking up named configurations and resolving variables or `undefined` for a non-folder setup. |
`nameOrConfiguration` | string \| [DebugConfiguration](../interfaces/_index_d_._plugin_.debugconfiguration.md) | Either the name of a debug or compound configuration or a [DebugConfiguration](#DebugConfiguration) object. |
`parentSessionOrOptions?` | [DebugSession](../interfaces/_index_d_._plugin_.debugsession.md) \| [DebugSessionOptions](../interfaces/_index_d_._plugin_.debugsessionoptions.md) | Debug sesison options. When passed a parent [debug session](#DebugSession), assumes options with just this parent session. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<boolean>

A thenable that resolves when debugging could be successfully started.
