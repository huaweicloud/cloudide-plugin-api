[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FilePermission

# Enumeration: FilePermission

["@codearts/plugin"](../modules/_codearts_plugin_.md).FilePermission

## Table of contents

### Enumeration Members

- [Readonly](codearts_plugin_.FilePermission.md#readonly)

## Enumeration Members

### Readonly

• **Readonly** = ``1``

The file is readonly.

*Note:* All `FileStat` from a `FileSystemProvider` that is registered with
the option `isReadonly: true` will be implicitly handled as if `FilePermission.Readonly`
is set. As a consequence, it is not possible to have a readonly file system provider
registered where some `FileStat` are not readonly.

#### Defined in

[index.d.ts:7800](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L7800)
