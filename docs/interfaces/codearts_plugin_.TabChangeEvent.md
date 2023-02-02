[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TabChangeEvent

# Interface: TabChangeEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).TabChangeEvent

An event describing change to tabs.

## Table of contents

### Properties

- [changed](codearts_plugin_.TabChangeEvent.md#changed)
- [closed](codearts_plugin_.TabChangeEvent.md#closed)
- [opened](codearts_plugin_.TabChangeEvent.md#opened)

## Properties

### changed

• `Readonly` **changed**: readonly [`Tab`](codearts_plugin_.Tab.md)[]

Tabs that have changed, e.g have changed
their [active](codearts_plugin_.Tab.md#isactive) state.

#### Defined in

[index.d.ts:16471](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16471)

___

### closed

• `Readonly` **closed**: readonly [`Tab`](codearts_plugin_.Tab.md)[]

The tabs that have been closed.

#### Defined in

[index.d.ts:16466](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16466)

___

### opened

• `Readonly` **opened**: readonly [`Tab`](codearts_plugin_.Tab.md)[]

The tabs that have been opened.

#### Defined in

[index.d.ts:16462](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16462)
