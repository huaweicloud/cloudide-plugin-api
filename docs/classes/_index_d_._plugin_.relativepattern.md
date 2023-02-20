**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / RelativePattern

# Class: RelativePattern

A relative pattern is a helper to construct glob patterns that are matched
relatively to a base file path. The base path can either be an absolute file
path as string or uri or a [workspace folder](#WorkspaceFolder), which is the
preferred way of creating the relative pattern.

## Hierarchy

* **RelativePattern**

## Index

### Constructors

* [constructor](_index_d_._plugin_.relativepattern.md#constructor)

### Properties

* [base](_index_d_._plugin_.relativepattern.md#base)
* [pattern](_index_d_._plugin_.relativepattern.md#pattern)

## Constructors

### constructor

\+ **new RelativePattern**(`base`: [WorkspaceFolder](../interfaces/_index_d_._plugin_.workspacefolder.md) \| [Uri](_index_d_._plugin_.uri.md) \| string, `pattern`: string): [RelativePattern](_index_d_._plugin_.relativepattern.md)

*Defined in [index.d.ts:2035](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L2035)*

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

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`base` | [WorkspaceFolder](../interfaces/_index_d_._plugin_.workspacefolder.md) \| [Uri](_index_d_._plugin_.uri.md) \| string | A base to which this pattern will be matched against relatively. It is recommended to pass in a [workspace folder](#WorkspaceFolder) if the pattern should match inside the workspace. Otherwise, a uri or string should only be used if the pattern is for a file path outside the workspace. |
`pattern` | string | A file glob pattern like `*.{ts,js}` that will be matched on paths relative to the base.  |

**Returns:** [RelativePattern](_index_d_._plugin_.relativepattern.md)

## Properties

### base

•  **base**: string

*Defined in [index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L2026)*

A base file path to which this pattern will be matched against relatively.

___

### pattern

•  **pattern**: string

*Defined in [index.d.ts:2035](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L2035)*

A file glob pattern like `*.{ts,js}` that will be matched on file paths
relative to the base path.

Example: Given a base of `/home/work/folder` and a file path of `/home/work/folder/index.js`,
the file glob pattern will match on `index.js`.
