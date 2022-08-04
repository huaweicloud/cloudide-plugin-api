[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TerminalOptions

# Interface: TerminalOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).TerminalOptions

## Table of contents

### Properties

- [color](codearts_plugin_.TerminalOptions.md#color)
- [cwd](codearts_plugin_.TerminalOptions.md#cwd)
- [env](codearts_plugin_.TerminalOptions.md#env)
- [hideFromUser](codearts_plugin_.TerminalOptions.md#hidefromuser)
- [iconPath](codearts_plugin_.TerminalOptions.md#iconpath)
- [isTransient](codearts_plugin_.TerminalOptions.md#istransient)
- [location](codearts_plugin_.TerminalOptions.md#location)
- [message](codearts_plugin_.TerminalOptions.md#message)
- [name](codearts_plugin_.TerminalOptions.md#name)
- [shellArgs](codearts_plugin_.TerminalOptions.md#shellargs)
- [shellPath](codearts_plugin_.TerminalOptions.md#shellpath)
- [strictEnv](codearts_plugin_.TerminalOptions.md#strictenv)

## Properties

### color

• `Optional` **color**: [`ThemeColor`](../classes/codearts_plugin_.ThemeColor.md)

#### Defined in

[index.d.ts:10526](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10526)

___

### cwd

• `Optional` **cwd**: `string` \| [`Uri`](../classes/codearts_plugin_.Uri.md)

#### Defined in

[index.d.ts:10484](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10484)

___

### env

• `Optional` **env**: `Object`

#### Index signature

▪ [key: `string`]: `string` \| ``null`` \| `undefined`

#### Defined in

[index.d.ts:10489](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10489)

___

### hideFromUser

• `Optional` **hideFromUser**: `boolean`

#### Defined in

[index.d.ts:10507](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10507)

___

### iconPath

• `Optional` **iconPath**: [`Uri`](../classes/codearts_plugin_.Uri.md) \| [`ThemeIcon`](../classes/codearts_plugin_.ThemeIcon.md) \| { `dark`: [`Uri`](../classes/codearts_plugin_.Uri.md) ; `light`: [`Uri`](../classes/codearts_plugin_.Uri.md)  }

#### Defined in

[index.d.ts:10519](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10519)

___

### isTransient

• `Optional` **isTransient**: `boolean`

#### Defined in

[index.d.ts:10537](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10537)

___

### location

• `Optional` **location**: [`TerminalEditorLocationOptions`](codearts_plugin_.TerminalEditorLocationOptions.md) \| [`TerminalSplitLocationOptions`](codearts_plugin_.TerminalSplitLocationOptions.md) \| [`TerminalLocation`](../enums/codearts_plugin_.TerminalLocation.md)

#### Defined in

[index.d.ts:10531](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10531)

___

### message

• `Optional` **message**: `string`

#### Defined in

[index.d.ts:10514](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10514)

___

### name

• `Optional` **name**: `string`

#### Defined in

[index.d.ts:10468](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10468)

___

### shellArgs

• `Optional` **shellArgs**: `string` \| `string`[]

#### Defined in

[index.d.ts:10479](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10479)

___

### shellPath

• `Optional` **shellPath**: `string`

#### Defined in

[index.d.ts:10473](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10473)

___

### strictEnv

• `Optional` **strictEnv**: `boolean`

#### Defined in

[index.d.ts:10498](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10498)
