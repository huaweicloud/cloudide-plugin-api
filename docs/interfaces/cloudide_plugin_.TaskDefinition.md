[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TaskDefinition

# Interface: TaskDefinition

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TaskDefinition

## Indexable

▪ [name: `string`]: `any`

## Table of contents

### Properties

- [type](cloudide_plugin_.TaskDefinition.md#type)

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

[index.d.ts:10375](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10375)
