[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TabGroupChangeEvent

# Interface: TabGroupChangeEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).TabGroupChangeEvent

An event describing changes to tab groups.

## Table of contents

### Properties

- [changed](codearts_plugin_.TabGroupChangeEvent.md#changed)
- [closed](codearts_plugin_.TabGroupChangeEvent.md#closed)
- [opened](codearts_plugin_.TabGroupChangeEvent.md#opened)

## Properties

### changed

• `Readonly` **changed**: readonly [`TabGroup`](codearts_plugin_.TabGroup.md)[]

Tab groups that have changed, e.g have changed
their [active](codearts_plugin_.TabGroup.md#isactive) state.

#### Defined in

[index.d.ts:17197](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17197)

___

### closed

• `Readonly` **closed**: readonly [`TabGroup`](codearts_plugin_.TabGroup.md)[]

Tab groups that have been closed.

#### Defined in

[index.d.ts:17192](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17192)

___

### opened

• `Readonly` **opened**: readonly [`TabGroup`](codearts_plugin_.TabGroup.md)[]

Tab groups that have been opened.

#### Defined in

[index.d.ts:17188](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17188)
