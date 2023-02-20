**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / ProgressLocation

# Enumeration: ProgressLocation

A location in the editor at which progress information can be shown. It depends on the
location how progress is visually represented.

## Index

### Enumeration members

* [Notification](_index_d_._plugin_.progresslocation.md#notification)
* [SourceControl](_index_d_._plugin_.progresslocation.md#sourcecontrol)
* [Window](_index_d_._plugin_.progresslocation.md#window)

## Enumeration members

### Notification

•  **Notification**:  = 15

*Defined in [index.d.ts:9710](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L9710)*

Show progress as notification with an optional cancel button. Supports to show infinite and discrete progress.

___

### SourceControl

•  **SourceControl**:  = 1

*Defined in [index.d.ts:9700](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L9700)*

Show progress for the source control viewlet, as overlay for the icon and as progress bar
inside the viewlet (when visible). Neither supports cancellation nor discrete progress.

___

### Window

•  **Window**:  = 10

*Defined in [index.d.ts:9705](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L9705)*

Show progress in the status bar of the editor. Neither supports cancellation nor discrete progress.
