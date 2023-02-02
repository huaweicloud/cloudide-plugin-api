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

[index.d.ts:16490](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16490)

___

### closed

• `Readonly` **closed**: readonly [`TabGroup`](codearts_plugin_.TabGroup.md)[]

Tab groups that have been closed.

#### Defined in

[index.d.ts:16485](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16485)

___

### opened

• `Readonly` **opened**: readonly [`TabGroup`](codearts_plugin_.TabGroup.md)[]

Tab groups that have been opened.

#### Defined in

[index.d.ts:16481](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16481)
