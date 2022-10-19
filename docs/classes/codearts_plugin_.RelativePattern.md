[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / RelativePattern

# Class: RelativePattern

["@codearts/plugin"](../modules/_codearts_plugin_.md).RelativePattern

A relative pattern is a helper to construct glob patterns that are matched
relatively to a base file path. The base path can either be an absolute file
path as string or uri or a [workspace folder](../interfaces/codearts_plugin_.WorkspaceFolder.md), which is the
preferred way of creating the relative pattern.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.RelativePattern.md#constructor)

### Properties

- [base](codearts_plugin_.RelativePattern.md#base)
- [baseUri](codearts_plugin_.RelativePattern.md#baseuri)
- [pattern](codearts_plugin_.RelativePattern.md#pattern)

## Constructors

### constructor

• **new RelativePattern**(`base`, `pattern`)

Creates a new relative pattern object with a base file path and pattern to match. This pattern
will be matched on file paths relative to the base.

Example:
```ts
const folder = vscode.workspace.workspaceFolders?.[0];
if (folder) {

  // Match any TypeScript file in the root of this workspace folder
  const pattern1 = new vscode.RelativePattern(folder, '*.ts');

  // Match any TypeScript file in `someFolder` inside this workspace folder
  const pattern2 = new vscode.RelativePattern(folder, 'someFolder/*.ts');
}
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `base` | `string` \| [`Uri`](codearts_plugin_.Uri.md) \| [`WorkspaceFolder`](../interfaces/codearts_plugin_.WorkspaceFolder.md) | A base to which this pattern will be matched against relatively. It is recommended to pass in a [workspace folder](../interfaces/codearts_plugin_.WorkspaceFolder.md) if the pattern should match inside the workspace. Otherwise, a uri or string should only be used if the pattern is for a file path outside the workspace. |
| `pattern` | `string` | A file glob pattern like `*.{ts,js}` that will be matched on paths relative to the base. |

#### Defined in

[index.d.ts:2124](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L2124)

## Properties

### base

• **base**: `string`

A base file path to which this pattern will be matched against relatively.

This matches the `fsPath` value of [baseUri](codearts_plugin_.RelativePattern.md#baseuri).

*Note:* updating this value will update [baseUri](codearts_plugin_.RelativePattern.md#baseuri) to
be a uri with `file` scheme.

**`Deprecated`**

This property is deprecated, please use [baseUri](codearts_plugin_.RelativePattern.md#baseuri) instead.

#### Defined in

[index.d.ts:2091](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L2091)

___

### baseUri

• **baseUri**: [`Uri`](codearts_plugin_.Uri.md)

A base file path to which this pattern will be matched against relatively.

#### Defined in

[index.d.ts:2079](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L2079)

___

### pattern

• **pattern**: `string`

A file glob pattern like `*.{ts,js}` that will be matched on file paths
relative to the base path.

Example: Given a base of `/home/work/folder` and a file path of `/home/work/folder/index.js`,
the file glob pattern will match on `index.js`.

#### Defined in

[index.d.ts:2100](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L2100)
