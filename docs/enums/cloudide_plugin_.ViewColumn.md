[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / ViewColumn

# Enumeration: ViewColumn

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).ViewColumn

Denotes a location of an editor in the window. Editors can be arranged in a grid
and each column represents one editor location in that grid by counting the editors
in order of their appearance.

## Table of contents

### Enumeration Members

- [Active](cloudide_plugin_.ViewColumn.md#active)
- [Beside](cloudide_plugin_.ViewColumn.md#beside)
- [Eight](cloudide_plugin_.ViewColumn.md#eight)
- [Five](cloudide_plugin_.ViewColumn.md#five)
- [Four](cloudide_plugin_.ViewColumn.md#four)
- [Nine](cloudide_plugin_.ViewColumn.md#nine)
- [One](cloudide_plugin_.ViewColumn.md#one)
- [Seven](cloudide_plugin_.ViewColumn.md#seven)
- [Six](cloudide_plugin_.ViewColumn.md#six)
- [Three](cloudide_plugin_.ViewColumn.md#three)
- [Two](cloudide_plugin_.ViewColumn.md#two)

## Enumeration Members

### Active

• **Active** = ``-1``

A *symbolic* editor column representing the currently active column. This value
can be used when opening editors, but the *resolved* [viewColumn](#TextEditor.viewColumn)-value
of editors will always be `One`, `Two`, `Three`,... or `undefined` but never `Active`.

#### Defined in

[index.d.ts:1969](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1969)

___

### Beside

• **Beside** = ``-2``

A *symbolic* editor column representing the column to the side of the active one. This value
can be used when opening editors, but the *resolved* [viewColumn](#TextEditor.viewColumn)-value
of editors will always be `One`, `Two`, `Three`,... or `undefined` but never `Beside`.

#### Defined in

[index.d.ts:1975](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1975)

___

### Eight

• **Eight** = ``8``

The eighth editor column.

#### Defined in

[index.d.ts:2007](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2007)

___

### Five

• **Five** = ``5``

The fifth editor column.

#### Defined in

[index.d.ts:1995](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1995)

___

### Four

• **Four** = ``4``

The fourth editor column.

#### Defined in

[index.d.ts:1991](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1991)

___

### Nine

• **Nine** = ``9``

The ninth editor column.

#### Defined in

[index.d.ts:2011](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2011)

___

### One

• **One** = ``1``

The first editor column.

#### Defined in

[index.d.ts:1979](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1979)

___

### Seven

• **Seven** = ``7``

The seventh editor column.

#### Defined in

[index.d.ts:2003](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2003)

___

### Six

• **Six** = ``6``

The sixth editor column.

#### Defined in

[index.d.ts:1999](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1999)

___

### Three

• **Three** = ``3``

The third editor column.

#### Defined in

[index.d.ts:1987](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1987)

___

### Two

• **Two** = ``2``

The second editor column.

#### Defined in

[index.d.ts:1983](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1983)
