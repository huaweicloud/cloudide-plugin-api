[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ViewColumn

# Enumeration: ViewColumn

["@codearts/plugin"](../modules/_codearts_plugin_.md).ViewColumn

Denotes a location of an editor in the window. Editors can be arranged in a grid
and each column represents one editor location in that grid by counting the editors
in order of their appearance.

## Table of contents

### Enumeration Members

- [Active](codearts_plugin_.ViewColumn.md#active)
- [Beside](codearts_plugin_.ViewColumn.md#beside)
- [Eight](codearts_plugin_.ViewColumn.md#eight)
- [Five](codearts_plugin_.ViewColumn.md#five)
- [Four](codearts_plugin_.ViewColumn.md#four)
- [Nine](codearts_plugin_.ViewColumn.md#nine)
- [One](codearts_plugin_.ViewColumn.md#one)
- [Seven](codearts_plugin_.ViewColumn.md#seven)
- [Six](codearts_plugin_.ViewColumn.md#six)
- [Three](codearts_plugin_.ViewColumn.md#three)
- [Two](codearts_plugin_.ViewColumn.md#two)

## Enumeration Members

### Active

• **Active** = ``-1``

A *symbolic* editor column representing the currently active column. This value
can be used when opening editors, but the *resolved* [viewColumn](../interfaces/codearts_plugin_.TextEditor.md#viewcolumn)-value
of editors will always be `One`, `Two`, `Three`,... or `undefined` but never `Active`.

#### Defined in

[index.d.ts:6250](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6250)

___

### Beside

• **Beside** = ``-2``

A *symbolic* editor column representing the column to the side of the active one. This value
can be used when opening editors, but the *resolved* [viewColumn](../interfaces/codearts_plugin_.TextEditor.md#viewcolumn)-value
of editors will always be `One`, `Two`, `Three`,... or `undefined` but never `Beside`.

#### Defined in

[index.d.ts:6256](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6256)

___

### Eight

• **Eight** = ``8``

The eighth editor column.

#### Defined in

[index.d.ts:6288](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6288)

___

### Five

• **Five** = ``5``

The fifth editor column.

#### Defined in

[index.d.ts:6276](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6276)

___

### Four

• **Four** = ``4``

The fourth editor column.

#### Defined in

[index.d.ts:6272](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6272)

___

### Nine

• **Nine** = ``9``

The ninth editor column.

#### Defined in

[index.d.ts:6292](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6292)

___

### One

• **One** = ``1``

The first editor column.

#### Defined in

[index.d.ts:6260](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6260)

___

### Seven

• **Seven** = ``7``

The seventh editor column.

#### Defined in

[index.d.ts:6284](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6284)

___

### Six

• **Six** = ``6``

The sixth editor column.

#### Defined in

[index.d.ts:6280](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6280)

___

### Three

• **Three** = ``3``

The third editor column.

#### Defined in

[index.d.ts:6268](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6268)

___

### Two

• **Two** = ``2``

The second editor column.

#### Defined in

[index.d.ts:6264](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6264)
