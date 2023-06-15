[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TestRun

# Interface: TestRun

["@codearts/plugin"](../modules/_codearts_plugin_.md).TestRun

Options given to TestController.runTests

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

Whether the test run will be persisted across reloads by the editor.

#### Defined in

[index.d.ts:16481](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16481)

___

### name

• `Readonly` **name**: `undefined` \| `string`

The human-readable name of the run. This can be used to
disambiguate multiple sets of results in a test run. It is useful if
tests are run across multiple platforms, for example.

#### Defined in

[index.d.ts:16470](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16470)

___

### token

• `Readonly` **token**: [`CancellationToken`](codearts_plugin_.CancellationToken.md)

A cancellation token which will be triggered when the test run is
canceled from the UI.

#### Defined in

[index.d.ts:16476](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16476)

## Methods

### appendOutput

▸ **appendOutput**(`output`, `location?`, `test?`): `void`

Appends raw output from the test runner. On the user's request, the
output will be displayed in a terminal. ANSI escape sequences,
such as colors and text styles, are supported.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `output` | `string` | Output text to append. |
| `location?` | [`Location`](../classes/codearts_plugin_.Location.md) | Indicate that the output was logged at the given location. |
| `test?` | [`TestItem`](codearts_plugin_.TestItem.md) | Test item to associate the output with. |

#### Returns

`void`

#### Defined in

[index.d.ts:16539](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16539)

___

### end

▸ **end**(): `void`

Signals that the end of the test run. Any tests included in the run whose
states have not been updated will have their state reset.

#### Returns

`void`

#### Defined in

[index.d.ts:16545](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16545)

___

### enqueued

▸ **enqueued**(`test`): `void`

Indicates a test is queued for later execution.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `test` | [`TestItem`](codearts_plugin_.TestItem.md) | Test item to update. |

#### Returns

`void`

#### Defined in

[index.d.ts:16487](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16487)

___

### errored

▸ **errored**(`test`, `message`, `duration?`): `void`

Indicates a test has errored. You should pass one or more
[TestMessages](../classes/codearts_plugin_.TestMessage.md) to describe the failure. This differs
from the "failed" state in that it indicates a test that couldn't be
executed at all, from a compilation error for example.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `test` | [`TestItem`](codearts_plugin_.TestItem.md) | Test item to update. |
| `message` | [`TestMessage`](../classes/codearts_plugin_.TestMessage.md) \| readonly [`TestMessage`](../classes/codearts_plugin_.TestMessage.md)[] | Messages associated with the test failure. |
| `duration?` | `number` | How long the test took to execute, in milliseconds. |

#### Returns

`void`

#### Defined in

[index.d.ts:16519](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16519)

___

### failed

▸ **failed**(`test`, `message`, `duration?`): `void`

Indicates a test has failed. You should pass one or more
[TestMessages](../classes/codearts_plugin_.TestMessage.md) to describe the failure.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `test` | [`TestItem`](codearts_plugin_.TestItem.md) | Test item to update. |
| `message` | [`TestMessage`](../classes/codearts_plugin_.TestMessage.md) \| readonly [`TestMessage`](../classes/codearts_plugin_.TestMessage.md)[] | Messages associated with the test failure. |
| `duration?` | `number` | How long the test took to execute, in milliseconds. |

#### Returns

`void`

#### Defined in

[index.d.ts:16508](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16508)

___

### passed

▸ **passed**(`test`, `duration?`, `message?`): `void`

Indicates a test has passed.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `test` | [`TestItem`](codearts_plugin_.TestItem.md) | Test item to update. |
| `duration?` | `number` | How long the test took to execute, in milliseconds. |
| `message?` | [`TestMessage`](../classes/codearts_plugin_.TestMessage.md) \| readonly [`TestMessage`](../classes/codearts_plugin_.TestMessage.md)[] | Messages associated with the test. |

#### Returns

`void`

#### Defined in

[index.d.ts:16527](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16527)

___

### skipped

▸ **skipped**(`test`): `void`

Indicates a test has been skipped.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `test` | [`TestItem`](codearts_plugin_.TestItem.md) | Test item to update. |

#### Returns

`void`

#### Defined in

[index.d.ts:16499](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16499)

___

### started

▸ **started**(`test`): `void`

Indicates a test has started running.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `test` | [`TestItem`](codearts_plugin_.TestItem.md) | Test item to update. |

#### Returns

`void`

#### Defined in

[index.d.ts:16493](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16493)
