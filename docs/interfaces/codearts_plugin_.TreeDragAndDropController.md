[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TreeDragAndDropController

# Interface: TreeDragAndDropController<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).TreeDragAndDropController

Provides support for drag and drop in `TreeView`.

## Type parameters

| Name |
| :------ |
| `T` |

## Table of contents

### Properties

- [dragMimeTypes](codearts_plugin_.TreeDragAndDropController.md#dragmimetypes)
- [dropMimeTypes](codearts_plugin_.TreeDragAndDropController.md#dropmimetypes)

### Methods

- [handleDrag](codearts_plugin_.TreeDragAndDropController.md#handledrag)
- [handleDrop](codearts_plugin_.TreeDragAndDropController.md#handledrop)

## Properties

### dragMimeTypes

• `Readonly` **dragMimeTypes**: readonly `string`[]

The mime types that the [`handleDrag`](codearts_plugin_.TreeDragAndDropController.md#handledrag) method of this `TreeDragAndDropController` may add to the tree data transfer.
This could be well-defined, existing, mime types, and also mime types defined by the extension.

The recommended mime type of the tree (`application/vnd.code.tree.<treeidlowercase>`) will be automatically added.

#### Defined in

[index.d.ts:10711](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L10711)

___

### dropMimeTypes

• `Readonly` **dropMimeTypes**: readonly `string`[]

The mime types that the [`handleDrop`](codearts_plugin_.TreeDragAndDropController.md#handledrop) method of this `DragAndDropController` supports.
This could be well-defined, existing, mime types, and also mime types defined by the extension.

To support drops from trees, you will need to add the mime type of that tree.
This includes drops from within the same tree.
The mime type of a tree is recommended to be of the format `application/vnd.code.tree.<treeidlowercase>`.

Use the special `files` mime type to support all types of dropped files [files](codearts_plugin_.DataTransferFile.md), regardless of the file's actual mime type.

To learn the mime type of a dragged item:
1. Set up your `DragAndDropController`
2. Use the Developer: Set Log Level... command to set the level to "Debug"
3. Open the developer tools and drag the item with unknown mime type over your tree. The mime types will be logged to the developer console

Note that mime types that cannot be sent to the extension will be omitted.

#### Defined in

[index.d.ts:10703](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L10703)

## Methods

### handleDrag

▸ `Optional` **handleDrag**(`source`, `dataTransfer`, `token`): `void` \| [`Thenable`](Thenable.md)<`void`\>

When the user starts dragging items from this `DragAndDropController`, `handleDrag` will be called.
Extensions can use `handleDrag` to add their [`DataTransferItem`](../classes/codearts_plugin_.DataTransferItem.md) items to the drag and drop.

When the items are dropped on **another tree item** in **the same tree**, your `DataTransferItem` objects
will be preserved. Use the recommended mime type for the tree (`application/vnd.code.tree.<treeidlowercase>`) to add
tree objects in a data transfer. See the documentation for `DataTransferItem` for how best to take advantage of this.

To add a data transfer item that can be dragged into the editor, use the application specific mime type "text/uri-list".
The data for "text/uri-list" should be a string with `toString()`ed Uris separated by newlines. To specify a cursor position in the file,
set the Uri's fragment to `L3,5`, where 3 is the line number and 5 is the column number.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | readonly `T`[] | The source items for the drag and drop operation. |
| `dataTransfer` | [`DataTransfer`](../classes/codearts_plugin_.DataTransfer.md) | The data transfer associated with this drag. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token indicating that drag has been cancelled. |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:10729](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L10729)

___

### handleDrop

▸ `Optional` **handleDrop**(`target`, `dataTransfer`, `token`): `void` \| [`Thenable`](Thenable.md)<`void`\>

Called when a drag and drop action results in a drop on the tree that this `DragAndDropController` belongs to.

Extensions should fire [onDidChangeTreeData](codearts_plugin_.TreeDataProvider.md#ondidchangetreedata) for any elements that need to be refreshed.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `undefined` \| `T` | The target tree element that the drop is occurring on. When undefined, the target is the root. |
| `dataTransfer` | [`DataTransfer`](../classes/codearts_plugin_.DataTransfer.md) | The data transfer items of the source of the drag. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token indicating that the drop has been cancelled. |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:10740](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L10740)
