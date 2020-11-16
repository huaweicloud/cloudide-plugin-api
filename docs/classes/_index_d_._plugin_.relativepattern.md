**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / RelativePattern

# Class: RelativePattern

A relative pattern is a helper to construct glob patterns that are matched
relatively to a base path. The base path can either be an absolute file path
or a [workspace folder](#WorkspaceFolder).

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

\+ **new RelativePattern**(`base`: [WorkspaceFolder](../interfaces/_index_d_._plugin_.workspacefolder.md) \| string, `pattern`: string): [RelativePattern](_index_d_._plugin_.relativepattern.md)

*Defined in [index.d.ts:1878](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1878)*

Creates a new relative pattern object with a base path and pattern to match. This pattern
will be matched on file paths relative to the base path.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`base` | [WorkspaceFolder](../interfaces/_index_d_._plugin_.workspacefolder.md) \| string | A base file path to which this pattern will be matched against relatively. |
`pattern` | string | A file glob pattern like `*.{ts,js}` that will be matched on file paths relative to the base path.  |

**Returns:** [RelativePattern](_index_d_._plugin_.relativepattern.md)

## Properties

### base

•  **base**: string

*Defined in [index.d.ts:1869](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1869)*

A base file path to which this pattern will be matched against relatively.

___

### pattern

•  **pattern**: string

*Defined in [index.d.ts:1878](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1878)*

A file glob pattern like `*.{ts,js}` that will be matched on file paths
relative to the base path.

Example: Given a base of `/home/work/folder` and a file path of `/home/work/folder/index.js`,
the file glob pattern will match on `index.js`.
