[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TestRunRequest

# Class: TestRunRequest

["@codearts/plugin"](../modules/_codearts_plugin_.md).TestRunRequest

A TestRunRequest is a precursor to a [TestRun](../interfaces/codearts_plugin_.TestRun.md), which in turn is
created by passing a request to tests.runTests. The TestRunRequest
contains information about which tests should be run, which should not be
run, and how they are run (via the [profile](codearts_plugin_.TestRunRequest.md#profile)).

In general, TestRunRequests are created by the editor and pass to
[runHandler](../interfaces/codearts_plugin_.TestRunProfile.md#runhandler), however you can also create test
requests and runs outside of the `runHandler`.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.TestRunRequest.md#constructor)

### Properties

- [exclude](codearts_plugin_.TestRunRequest.md#exclude)
- [include](codearts_plugin_.TestRunRequest.md#include)
- [profile](codearts_plugin_.TestRunRequest.md#profile)

## Constructors

### constructor

• **new TestRunRequest**(`include?`, `exclude?`, `profile?`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `include?` | readonly [`TestItem`](../interfaces/codearts_plugin_.TestItem.md)[] | Array of specific tests to run, or undefined to run all tests |
| `exclude?` | readonly [`TestItem`](../interfaces/codearts_plugin_.TestItem.md)[] | An array of tests to exclude from the run. |
| `profile?` | [`TestRunProfile`](../interfaces/codearts_plugin_.TestRunProfile.md) | The run profile used for this request. |

#### Defined in

[index.d.ts:16406](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16406)

## Properties

### exclude

• `Readonly` **exclude**: `undefined` \| readonly [`TestItem`](../interfaces/codearts_plugin_.TestItem.md)[]

An array of tests the user has marked as excluded from the test included
in this run; exclusions should apply after inclusions.

May be omitted if no exclusions were requested. Test controllers should
not run excluded tests or any children of excluded tests.

#### Defined in

[index.d.ts:16392](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16392)

___

### include

• `Readonly` **include**: `undefined` \| readonly [`TestItem`](../interfaces/codearts_plugin_.TestItem.md)[]

A filter for specific tests to run. If given, the extension should run
all of the included tests and all their children, excluding any tests
that appear in [exclude](codearts_plugin_.TestRunRequest.md#exclude). If this property is
undefined, then the extension should simply run all tests.

The process of running tests should resolve the children of any test
items who have not yet been resolved.

#### Defined in

[index.d.ts:16383](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16383)

___

### profile

• `Readonly` **profile**: `undefined` \| [`TestRunProfile`](../interfaces/codearts_plugin_.TestRunProfile.md)

The profile used for this request. This will always be defined
for requests issued from the editor UI, though extensions may
programmatically create requests not associated with any profile.

#### Defined in

[index.d.ts:16399](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16399)
