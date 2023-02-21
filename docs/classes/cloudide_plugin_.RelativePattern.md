[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / RelativePattern

# Class: RelativePattern

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).RelativePattern

A relative pattern is a helper to construct glob patterns that are matched
relatively to a base path. The base path can either be an absolute file path
or a [workspace folder](#WorkspaceFolder).

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.RelativePattern.md#constructor)

### Properties

- [base](cloudide_plugin_.RelativePattern.md#base)
- [pattern](cloudide_plugin_.RelativePattern.md#pattern)

## Constructors

### constructor

• **new RelativePattern**(`base`, `pattern`)

Creates a new relative pattern object with a base path and pattern to match. This pattern
will be matched on file paths relative to the base path.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `base` | `string` \| [`WorkspaceFolder`](../interfaces/cloudide_plugin_.WorkspaceFolder.md) | A base file path to which this pattern will be matched against relatively. |
| `pattern` | `string` | A file glob pattern like `*.{ts,js}` that will be matched on file paths relative to the base path. |

#### Defined in

[index.d.ts:6522](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6522)

## Properties

### base

• **base**: `string`

A base file path to which this pattern will be matched against relatively.

#### Defined in

[index.d.ts:6503](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6503)

___

### pattern

• **pattern**: `string`

A file glob pattern like `*.{ts,js}` that will be matched on file paths
relative to the base path.

Example: Given a base of `/home/work/folder` and a file path of `/home/work/folder/index.js`,
the file glob pattern will match on `index.js`.

#### Defined in

[index.d.ts:6512](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6512)
