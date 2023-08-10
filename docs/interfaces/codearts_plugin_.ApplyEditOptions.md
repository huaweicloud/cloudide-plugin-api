[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ApplyEditOptions

# Interface: ApplyEditOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).ApplyEditOptions

## Table of contents

### Properties

- [code](codearts_plugin_.ApplyEditOptions.md#code)
- [confirmBeforeUndo](codearts_plugin_.ApplyEditOptions.md#confirmbeforeundo)
- [enableUndoFile](codearts_plugin_.ApplyEditOptions.md#enableundofile)
- [label](codearts_plugin_.ApplyEditOptions.md#label)
- [quotableLabel](codearts_plugin_.ApplyEditOptions.md#quotablelabel)
- [respectAutoSaveConfig](codearts_plugin_.ApplyEditOptions.md#respectautosaveconfig)
- [showPreview](codearts_plugin_.ApplyEditOptions.md#showpreview)

## Properties

### code

• `Optional` **code**: `string`

operation code.

#### Defined in

[index.d.ts:3481](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L3481)

___

### confirmBeforeUndo

• `Optional` **confirmBeforeUndo**: `boolean`

Controls whether the explorer should ask for confirmation when undoing. default false.

#### Defined in

[index.d.ts:3491](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L3491)

___

### enableUndoFile

• `Optional` **enableUndoFile**: `boolean`

Whether the file operations (create renameFile, deleteFile) on the working area can be undone.

#### Defined in

[index.d.ts:3471](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L3471)

___

### label

• `Optional` **label**: `string`

undo prompt showed text.

#### Defined in

[index.d.ts:3476](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L3476)

___

### quotableLabel

• `Optional` **quotableLabel**: `string`

Provides a referenceable tag so that users can reference it in different contexts. When there is a value, the label field is replaced.

#### Defined in

[index.d.ts:3486](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L3486)

___

### respectAutoSaveConfig

• `Optional` **respectAutoSaveConfig**: `boolean`

Controls whether auto-save configurations should be respected. default true.

#### Defined in

[index.d.ts:3496](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L3496)

___

### showPreview

• `Optional` **showPreview**: `boolean`

file opened type.

#### Defined in

[index.d.ts:3501](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L3501)
