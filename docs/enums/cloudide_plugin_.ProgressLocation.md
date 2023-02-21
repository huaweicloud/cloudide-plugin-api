[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / ProgressLocation

# Enumeration: ProgressLocation

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).ProgressLocation

A location in the editor at which progress information can be shown. It depends on the
location how progress is visually represented.

## Table of contents

### Enumeration Members

- [Notification](cloudide_plugin_.ProgressLocation.md#notification)
- [SourceControl](cloudide_plugin_.ProgressLocation.md#sourcecontrol)
- [Window](cloudide_plugin_.ProgressLocation.md#window)

## Enumeration Members

### Notification

• **Notification** = ``15``

Show progress as notification with an optional cancel button. Supports to show infinite and discrete progress.

#### Defined in

[index.d.ts:5137](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5137)

___

### SourceControl

• **SourceControl** = ``1``

Show progress for the source control viewlet, as overlay for the icon and as progress bar
inside the viewlet (when visible). Neither supports cancellation nor discrete progress.

#### Defined in

[index.d.ts:5129](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5129)

___

### Window

• **Window** = ``10``

Show progress in the status bar of the editor. Neither supports cancellation nor discrete progress.

#### Defined in

[index.d.ts:5133](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5133)
