[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextEditor

# Interface: TextEditor

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextEditor

## Table of contents

### Properties

- [document](codearts_plugin_.TextEditor.md#document)
- [options](codearts_plugin_.TextEditor.md#options)
- [selection](codearts_plugin_.TextEditor.md#selection)
- [selections](codearts_plugin_.TextEditor.md#selections)
- [viewColumn](codearts_plugin_.TextEditor.md#viewcolumn)
- [visibleRanges](codearts_plugin_.TextEditor.md#visibleranges)

### Methods

- [edit](codearts_plugin_.TextEditor.md#edit)
- [hide](codearts_plugin_.TextEditor.md#hide)
- [insertSnippet](codearts_plugin_.TextEditor.md#insertsnippet)
- [revealRange](codearts_plugin_.TextEditor.md#revealrange)
- [setDecorations](codearts_plugin_.TextEditor.md#setdecorations)
- [show](codearts_plugin_.TextEditor.md#show)

## Properties

### document

• `Readonly` **document**: [`TextDocument`](codearts_plugin_.TextDocument.md)

#### Defined in

[index.d.ts:1169](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L1169)

___

### options

• **options**: [`TextEditorOptions`](codearts_plugin_.TextEditorOptions.md)

#### Defined in

[index.d.ts:1190](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L1190)

___

### selection

• **selection**: [`Selection`](../classes/codearts_plugin_.Selection.md)

#### Defined in

[index.d.ts:1174](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L1174)

___

### selections

• **selections**: readonly [`Selection`](../classes/codearts_plugin_.Selection.md)[]

#### Defined in

[index.d.ts:1179](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L1179)

___

### viewColumn

• `Readonly` **viewColumn**: `undefined` \| [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md)

#### Defined in

[index.d.ts:1197](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L1197)

___

### visibleRanges

• `Readonly` **visibleRanges**: readonly [`Range`](../classes/codearts_plugin_.Range.md)[]

#### Defined in

[index.d.ts:1185](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L1185)

## Methods

### edit

▸ **edit**(`callback`, `options?`): [`Thenable`](Thenable.md)<`boolean`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`editBuilder`: [`TextEditorEdit`](codearts_plugin_.TextEditorEdit.md)) => `void` |  |
| `options?` | `Object` |  |
| `options.undoStopAfter` | `boolean` | - |
| `options.undoStopBefore` | `boolean` | - |

#### Returns

[`Thenable`](Thenable.md)<`boolean`\>

#### Defined in

[index.d.ts:1210](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L1210)

___

### hide

▸ **hide**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:1262](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L1262)

___

### insertSnippet

▸ **insertSnippet**(`snippet`, `location?`, `options?`): [`Thenable`](Thenable.md)<`boolean`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `snippet` | [`SnippetString`](../classes/codearts_plugin_.SnippetString.md) |  |
| `location?` | [`Range`](../classes/codearts_plugin_.Range.md) \| [`Position`](../classes/codearts_plugin_.Position.md) \| readonly [`Range`](../classes/codearts_plugin_.Range.md)[] \| readonly [`Position`](../classes/codearts_plugin_.Position.md)[] |  |
| `options?` | `Object` |  |
| `options.undoStopAfter` | `boolean` | - |
| `options.undoStopBefore` | `boolean` | - |

#### Returns

[`Thenable`](Thenable.md)<`boolean`\>

#### Defined in

[index.d.ts:1223](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L1223)

___

### revealRange

▸ **revealRange**(`range`, `revealType?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](../classes/codearts_plugin_.Range.md) |  |
| `revealType?` | [`TextEditorRevealType`](../enums/codearts_plugin_.TextEditorRevealType.md) |  |

#### Returns

`void`

#### Defined in

[index.d.ts:1244](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L1244)

___

### setDecorations

▸ **setDecorations**(`decorationType`, `rangesOrOptions`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `decorationType` | [`TextEditorDecorationType`](codearts_plugin_.TextEditorDecorationType.md) |  |
| `rangesOrOptions` | readonly [`Range`](../classes/codearts_plugin_.Range.md)[] \| readonly [`DecorationOptions`](codearts_plugin_.DecorationOptions.md)[] |  |

#### Returns

`void`

#### Defined in

[index.d.ts:1236](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L1236)

___

### show

▸ **show**(`column?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `column?` | [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md) |  |

#### Returns

`void`

#### Defined in

[index.d.ts:1254](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L1254)
