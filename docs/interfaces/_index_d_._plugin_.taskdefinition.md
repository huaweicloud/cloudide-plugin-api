**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TaskDefinition

# Interface: TaskDefinition

A structure that defines a task kind in the system.
The value must be JSON-stringifyable.

## Hierarchy

* **TaskDefinition**

## Indexable

▪ [name: string]: any

Additional attributes of a concrete task definition.

## Index

### Properties

* [type](_index_d_._plugin_.taskdefinition.md#type)

## Properties

### type

• `Readonly` **type**: string

*Defined in [index.d.ts:6284](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6284)*

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
