[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ProgressLocation

# Enumeration: ProgressLocation

["@codearts/plugin"](../modules/_codearts_plugin_.md).ProgressLocation

A location in the editor at which progress information can be shown. It depends on the
location how progress is visually represented.

## Table of contents

### Enumeration Members

- [Notification](codearts_plugin_.ProgressLocation.md#notification)
- [SourceControl](codearts_plugin_.ProgressLocation.md#sourcecontrol)
- [Window](codearts_plugin_.ProgressLocation.md#window)

## Enumeration Members

### Notification

• **Notification** = ``15``

Show progress as notification with an optional cancel button. Supports to show infinite and discrete
progress but does not support rendering of icons.

#### Defined in

[index.d.ts:11287](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L11287)

___

### SourceControl

• **SourceControl** = ``1``

Show progress for the source control viewlet, as overlay for the icon and as progress bar
inside the viewlet (when visible). Neither supports cancellation nor discrete progress nor
a label to describe the operation.

#### Defined in

[index.d.ts:11275](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L11275)

___

### Window

• **Window** = ``10``

Show progress in the status bar of the editor. Neither supports cancellation nor discrete progress.
Supports rendering of [theme icons](../classes/codearts_plugin_.ThemeIcon.md) via the `$(<name>)`-syntax in the progress label.

#### Defined in

[index.d.ts:11281](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L11281)
