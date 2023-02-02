[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TaskDefinition

# Interface: TaskDefinition

["@codearts/plugin"](../modules/_codearts_plugin_.md).TaskDefinition

A structure that defines a task kind in the system.
The value must be JSON-stringifyable.

## Indexable

▪ [name: `string`]: `any`

## Table of contents

### Properties

- [type](codearts_plugin_.TaskDefinition.md#type)

## Properties

### type

• `Readonly` **type**: `string`

The task definition describing the task provided by an extension.
Usually a task provider defines more properties to identify
a task. They need to be defined in the package.json of the
extension under the 'taskDefinitions' extension point. The npm
task definition for example looks like this
```typescript
interface NpmTaskDefinition extends TaskDefinition {
    script: string;
}
```

Note that type identifier starting with a '$' are reserved for internal
usages and shouldn't be used by extensions.

#### Defined in

[index.d.ts:7275](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L7275)
