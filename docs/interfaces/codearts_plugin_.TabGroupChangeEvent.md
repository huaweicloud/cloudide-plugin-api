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

[index.d.ts:17322](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17322)

___

### closed

• `Readonly` **closed**: readonly [`TabGroup`](codearts_plugin_.TabGroup.md)[]

Tab groups that have been closed.

#### Defined in

[index.d.ts:17317](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17317)

___

### opened

• `Readonly` **opened**: readonly [`TabGroup`](codearts_plugin_.TabGroup.md)[]

Tab groups that have been opened.

#### Defined in

[index.d.ts:17313](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17313)
