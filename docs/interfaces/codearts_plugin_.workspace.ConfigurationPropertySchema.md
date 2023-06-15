[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / [workspace](../modules/codearts_plugin_.workspace.md) / ConfigurationPropertySchema

# Interface: ConfigurationPropertySchema

["@codearts/plugin"](../modules/_codearts_plugin_.md).[workspace](../modules/codearts_plugin_.workspace.md).ConfigurationPropertySchema

## Hierarchy

- [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

  ↳ **`ConfigurationPropertySchema`**

## Table of contents

### Properties

- [$anchor](codearts_plugin_.workspace.ConfigurationPropertySchema.md#$anchor)
- [$comment](codearts_plugin_.workspace.ConfigurationPropertySchema.md#$comment)
- [$defs](codearts_plugin_.workspace.ConfigurationPropertySchema.md#$defs)
- [$dynamicAnchor](codearts_plugin_.workspace.ConfigurationPropertySchema.md#$dynamicanchor)
- [$dynamicRef](codearts_plugin_.workspace.ConfigurationPropertySchema.md#$dynamicref)
- [$id](codearts_plugin_.workspace.ConfigurationPropertySchema.md#$id)
- [$recursiveAnchor](codearts_plugin_.workspace.ConfigurationPropertySchema.md#$recursiveanchor)
- [$recursiveRef](codearts_plugin_.workspace.ConfigurationPropertySchema.md#$recursiveref)
- [$ref](codearts_plugin_.workspace.ConfigurationPropertySchema.md#$ref)
- [$schema](codearts_plugin_.workspace.ConfigurationPropertySchema.md#$schema)
- [$vocabulary](codearts_plugin_.workspace.ConfigurationPropertySchema.md#$vocabulary)
- [additionalItems](codearts_plugin_.workspace.ConfigurationPropertySchema.md#additionalitems)
- [additionalProperties](codearts_plugin_.workspace.ConfigurationPropertySchema.md#additionalproperties)
- [allOf](codearts_plugin_.workspace.ConfigurationPropertySchema.md#allof)
- [allowComments](codearts_plugin_.workspace.ConfigurationPropertySchema.md#allowcomments)
- [allowTrailingCommas](codearts_plugin_.workspace.ConfigurationPropertySchema.md#allowtrailingcommas)
- [anyOf](codearts_plugin_.workspace.ConfigurationPropertySchema.md#anyof)
- [browse](codearts_plugin_.workspace.ConfigurationPropertySchema.md#browse)
- [const](codearts_plugin_.workspace.ConfigurationPropertySchema.md#const)
- [contains](codearts_plugin_.workspace.ConfigurationPropertySchema.md#contains)
- [default](codearts_plugin_.workspace.ConfigurationPropertySchema.md#default)
- [defaultSnippets](codearts_plugin_.workspace.ConfigurationPropertySchema.md#defaultsnippets)
- [definitions](codearts_plugin_.workspace.ConfigurationPropertySchema.md#definitions)
- [dependencies](codearts_plugin_.workspace.ConfigurationPropertySchema.md#dependencies)
- [dependentRequired](codearts_plugin_.workspace.ConfigurationPropertySchema.md#dependentrequired)
- [dependentSchemas](codearts_plugin_.workspace.ConfigurationPropertySchema.md#dependentschemas)
- [deprecated](codearts_plugin_.workspace.ConfigurationPropertySchema.md#deprecated)
- [deprecationMessage](codearts_plugin_.workspace.ConfigurationPropertySchema.md#deprecationmessage)
- [description](codearts_plugin_.workspace.ConfigurationPropertySchema.md#description)
- [disallowSyncIgnore](codearts_plugin_.workspace.ConfigurationPropertySchema.md#disallowsyncignore)
- [doNotSuggest](codearts_plugin_.workspace.ConfigurationPropertySchema.md#donotsuggest)
- [editPresentation](codearts_plugin_.workspace.ConfigurationPropertySchema.md#editpresentation)
- [else](codearts_plugin_.workspace.ConfigurationPropertySchema.md#else)
- [enum](codearts_plugin_.workspace.ConfigurationPropertySchema.md#enum)
- [enumDescriptions](codearts_plugin_.workspace.ConfigurationPropertySchema.md#enumdescriptions)
- [enumItemLabels](codearts_plugin_.workspace.ConfigurationPropertySchema.md#enumitemlabels)
- [errorMessage](codearts_plugin_.workspace.ConfigurationPropertySchema.md#errormessage)
- [examples](codearts_plugin_.workspace.ConfigurationPropertySchema.md#examples)
- [exclusiveMaximum](codearts_plugin_.workspace.ConfigurationPropertySchema.md#exclusivemaximum)
- [exclusiveMinimum](codearts_plugin_.workspace.ConfigurationPropertySchema.md#exclusiveminimum)
- [format](codearts_plugin_.workspace.ConfigurationPropertySchema.md#format)
- [id](codearts_plugin_.workspace.ConfigurationPropertySchema.md#id)
- [if](codearts_plugin_.workspace.ConfigurationPropertySchema.md#if)
- [ignoreSync](codearts_plugin_.workspace.ConfigurationPropertySchema.md#ignoresync)
- [included](codearts_plugin_.workspace.ConfigurationPropertySchema.md#included)
- [items](codearts_plugin_.workspace.ConfigurationPropertySchema.md#items)
- [markdownDeprecationMessage](codearts_plugin_.workspace.ConfigurationPropertySchema.md#markdowndeprecationmessage)
- [markdownDescription](codearts_plugin_.workspace.ConfigurationPropertySchema.md#markdowndescription)
- [markdownEnumDescriptions](codearts_plugin_.workspace.ConfigurationPropertySchema.md#markdownenumdescriptions)
- [maxContains](codearts_plugin_.workspace.ConfigurationPropertySchema.md#maxcontains)
- [maxItems](codearts_plugin_.workspace.ConfigurationPropertySchema.md#maxitems)
- [maxLength](codearts_plugin_.workspace.ConfigurationPropertySchema.md#maxlength)
- [maxProperties](codearts_plugin_.workspace.ConfigurationPropertySchema.md#maxproperties)
- [maximum](codearts_plugin_.workspace.ConfigurationPropertySchema.md#maximum)
- [minContains](codearts_plugin_.workspace.ConfigurationPropertySchema.md#mincontains)
- [minItems](codearts_plugin_.workspace.ConfigurationPropertySchema.md#minitems)
- [minLength](codearts_plugin_.workspace.ConfigurationPropertySchema.md#minlength)
- [minProperties](codearts_plugin_.workspace.ConfigurationPropertySchema.md#minproperties)
- [minimum](codearts_plugin_.workspace.ConfigurationPropertySchema.md#minimum)
- [multipleOf](codearts_plugin_.workspace.ConfigurationPropertySchema.md#multipleof)
- [not](codearts_plugin_.workspace.ConfigurationPropertySchema.md#not)
- [oneOf](codearts_plugin_.workspace.ConfigurationPropertySchema.md#oneof)
- [order](codearts_plugin_.workspace.ConfigurationPropertySchema.md#order)
- [pattern](codearts_plugin_.workspace.ConfigurationPropertySchema.md#pattern)
- [patternErrorMessage](codearts_plugin_.workspace.ConfigurationPropertySchema.md#patternerrormessage)
- [patternProperties](codearts_plugin_.workspace.ConfigurationPropertySchema.md#patternproperties)
- [policy](codearts_plugin_.workspace.ConfigurationPropertySchema.md#policy)
- [prefixItems](codearts_plugin_.workspace.ConfigurationPropertySchema.md#prefixitems)
- [properties](codearts_plugin_.workspace.ConfigurationPropertySchema.md#properties)
- [propertyNames](codearts_plugin_.workspace.ConfigurationPropertySchema.md#propertynames)
- [required](codearts_plugin_.workspace.ConfigurationPropertySchema.md#required)
- [restricted](codearts_plugin_.workspace.ConfigurationPropertySchema.md#restricted)
- [scope](codearts_plugin_.workspace.ConfigurationPropertySchema.md#scope)
- [subTitle](codearts_plugin_.workspace.ConfigurationPropertySchema.md#subtitle)
- [suggestSortText](codearts_plugin_.workspace.ConfigurationPropertySchema.md#suggestsorttext)
- [tags](codearts_plugin_.workspace.ConfigurationPropertySchema.md#tags)
- [then](codearts_plugin_.workspace.ConfigurationPropertySchema.md#then)
- [title](codearts_plugin_.workspace.ConfigurationPropertySchema.md#title)
- [type](codearts_plugin_.workspace.ConfigurationPropertySchema.md#type)
- [unevaluatedItems](codearts_plugin_.workspace.ConfigurationPropertySchema.md#unevaluateditems)
- [unevaluatedProperties](codearts_plugin_.workspace.ConfigurationPropertySchema.md#unevaluatedproperties)
- [uniqueItems](codearts_plugin_.workspace.ConfigurationPropertySchema.md#uniqueitems)

## Properties

### $anchor

• `Optional` **$anchor**: `string`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[$anchor](codearts_plugin_.workspace.JSONSchema.md#$anchor)

#### Defined in

[index.d.ts:12908](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12908)

___

### $comment

• `Optional` **$comment**: `string`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[$comment](codearts_plugin_.workspace.JSONSchema.md#$comment)

#### Defined in

[index.d.ts:12896](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12896)

___

### $defs

• `Optional` **$defs**: `Object`

#### Index signature

▪ [name: `string`]: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[$defs](codearts_plugin_.workspace.JSONSchema.md#$defs)

#### Defined in

[index.d.ts:12907](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12907)

___

### $dynamicAnchor

• `Optional` **$dynamicAnchor**: `string`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[$dynamicAnchor](codearts_plugin_.workspace.JSONSchema.md#$dynamicanchor)

#### Defined in

[index.d.ts:12914](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12914)

___

### $dynamicRef

• `Optional` **$dynamicRef**: `string`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[$dynamicRef](codearts_plugin_.workspace.JSONSchema.md#$dynamicref)

#### Defined in

[index.d.ts:12913](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12913)

___

### $id

• `Optional` **$id**: `string`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[$id](codearts_plugin_.workspace.JSONSchema.md#$id)

#### Defined in

[index.d.ts:12798](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12798)

___

### $recursiveAnchor

• `Optional` **$recursiveAnchor**: `string`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[$recursiveAnchor](codearts_plugin_.workspace.JSONSchema.md#$recursiveanchor)

#### Defined in

[index.d.ts:12910](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12910)

___

### $recursiveRef

• `Optional` **$recursiveRef**: `string`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[$recursiveRef](codearts_plugin_.workspace.JSONSchema.md#$recursiveref)

#### Defined in

[index.d.ts:12909](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12909)

___

### $ref

• `Optional` **$ref**: `string`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[$ref](codearts_plugin_.workspace.JSONSchema.md#$ref)

#### Defined in

[index.d.ts:12881](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12881)

___

### $schema

• `Optional` **$schema**: `string`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[$schema](codearts_plugin_.workspace.JSONSchema.md#$schema)

#### Defined in

[index.d.ts:12799](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12799)

___

### $vocabulary

• `Optional` **$vocabulary**: `any`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[$vocabulary](codearts_plugin_.workspace.JSONSchema.md#$vocabulary)

#### Defined in

[index.d.ts:12911](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12911)

___

### additionalItems

• `Optional` **additionalItems**: `boolean` \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[additionalItems](codearts_plugin_.workspace.JSONSchema.md#additionalitems)

#### Defined in

[index.d.ts:12851](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12851)

___

### additionalProperties

• `Optional` **additionalProperties**: `boolean` \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

[`additionalProperties`](codearts_plugin_.workspace.ConfigurationPropertySchema.md#additionalproperties)ConfigurationType
Either a schema or a boolean. If a schema, then used to validate all properties not matched by 'properties' or 'patternProperties'.
If false, then any properties not matched by either will cause this schema to fail.

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[additionalProperties](codearts_plugin_.workspace.JSONSchema.md#additionalproperties)

#### Defined in

[index.d.ts:12835](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12835)

___

### allOf

• `Optional` **allOf**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[allOf](codearts_plugin_.workspace.JSONSchema.md#allof)

#### Defined in

[index.d.ts:12883](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12883)

___

### allowComments

• `Optional` **allowComments**: `boolean`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[allowComments](codearts_plugin_.workspace.JSONSchema.md#allowcomments)

#### Defined in

[index.d.ts:12929](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12929)

___

### allowTrailingCommas

• `Optional` **allowTrailingCommas**: `boolean`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[allowTrailingCommas](codearts_plugin_.workspace.JSONSchema.md#allowtrailingcommas)

#### Defined in

[index.d.ts:12930](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12930)

___

### anyOf

• `Optional` **anyOf**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[anyOf](codearts_plugin_.workspace.JSONSchema.md#anyof)

#### Defined in

[index.d.ts:12882](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12882)

___

### browse

• `Optional` **browse**: [`ConfigurationBrowseType`](../enums/codearts_plugin_.ConfigurationBrowseType.md)

"file" | "folder"

#### Defined in

[index.d.ts:12793](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12793)

___

### const

• `Optional` **const**: `any`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[const](codearts_plugin_.workspace.JSONSchema.md#const)

#### Defined in

[index.d.ts:12892](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12892)

___

### contains

• `Optional` **contains**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[contains](codearts_plugin_.workspace.JSONSchema.md#contains)

#### Defined in

[index.d.ts:12893](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12893)

___

### default

• `Optional` **default**: `any`

For defining the default value of a property.

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[default](codearts_plugin_.workspace.JSONSchema.md#default)

#### Defined in

[index.d.ts:12818](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12818)

___

### defaultSnippets

• `Optional` **defaultSnippets**: [`JSONSchemaSnippet`](codearts_plugin_.workspace.JSONSchemaSnippet.md)[]

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[defaultSnippets](codearts_plugin_.workspace.JSONSchema.md#defaultsnippets)

#### Defined in

[index.d.ts:12915](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12915)

___

### definitions

• `Optional` **definitions**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md)

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[definitions](codearts_plugin_.workspace.JSONSchema.md#definitions)

#### Defined in

[index.d.ts:12819](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12819)

___

### dependencies

• `Optional` **dependencies**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md) \| { `[prop: string]`: `string`[];  }

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[dependencies](codearts_plugin_.workspace.JSONSchema.md#dependencies)

#### Defined in

[index.d.ts:12838](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12838)

___

### dependentRequired

• `Optional` **dependentRequired**: `Object`

#### Index signature

▪ [prop: `string`]: `string`[]

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[dependentRequired](codearts_plugin_.workspace.JSONSchema.md#dependentrequired)

#### Defined in

[index.d.ts:12905](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12905)

___

### dependentSchemas

• `Optional` **dependentSchemas**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md)

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[dependentSchemas](codearts_plugin_.workspace.JSONSchema.md#dependentschemas)

#### Defined in

[index.d.ts:12906](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12906)

___

### deprecated

• `Optional` **deprecated**: `boolean`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[deprecated](codearts_plugin_.workspace.JSONSchema.md#deprecated)

#### Defined in

[index.d.ts:12904](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12904)

___

### deprecationMessage

• `Optional` **deprecationMessage**: `string`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[deprecationMessage](codearts_plugin_.workspace.JSONSchema.md#deprecationmessage)

#### Defined in

[index.d.ts:12922](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12922)

___

### description

• `Optional` **description**: `string`

Your description appears after the title and before the input field,
except for booleans, where the description is used as the label for the checkbox.
For markdownDescription, in order to add newlines or multiple paragraphs, use the string \n\n to separate the paragraphs instead of just \n.

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[description](codearts_plugin_.workspace.JSONSchema.md#description)

#### Defined in

[index.d.ts:12826](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12826)

___

### disallowSyncIgnore

• `Optional` **disallowSyncIgnore**: `boolean`

When enabled this setting is ignored during sync and user cannot override this.

#### Defined in

[index.d.ts:12765](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12765)

___

### doNotSuggest

• `Optional` **doNotSuggest**: `boolean`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[doNotSuggest](codearts_plugin_.workspace.JSONSchema.md#donotsuggest)

#### Defined in

[index.d.ts:12927](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12927)

___

### editPresentation

• `Optional` **editPresentation**: [`EditPresentationTypes`](../enums/codearts_plugin_.EditPresentationTypes.md)

When specified, controls the presentation format of string settings.
Otherwise, the presentation format defaults to `singleline`.

#### Defined in

[index.d.ts:12776](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12776)

___

### else

• `Optional` **else**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[else](codearts_plugin_.workspace.JSONSchema.md#else)

#### Defined in

[index.d.ts:12899](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12899)

___

### enum

• `Optional` **enum**: `any`[]

If you provide an array of items under the enum property, the settings UI will render a dropdown menu.

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[enum](codearts_plugin_.workspace.JSONSchema.md#enum)

#### Defined in

[index.d.ts:12890](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12890)

___

### enumDescriptions

• `Optional` **enumDescriptions**: `string`[]

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[enumDescriptions](codearts_plugin_.workspace.JSONSchema.md#enumdescriptions)

#### Defined in

[index.d.ts:12924](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12924)

___

### enumItemLabels

• `Optional` **enumItemLabels**: `string`[]

Labels for enumeration items

#### Defined in

[index.d.ts:12770](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12770)

___

### errorMessage

• `Optional` **errorMessage**: `string`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[errorMessage](codearts_plugin_.workspace.JSONSchema.md#errormessage)

#### Defined in

[index.d.ts:12916](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12916)

___

### examples

• `Optional` **examples**: `any`[]

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[examples](codearts_plugin_.workspace.JSONSchema.md#examples)

#### Defined in

[index.d.ts:12895](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12895)

___

### exclusiveMaximum

• `Optional` **exclusiveMaximum**: `number` \| `boolean`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[exclusiveMaximum](codearts_plugin_.workspace.JSONSchema.md#exclusivemaximum)

#### Defined in

[index.d.ts:12878](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12878)

___

### exclusiveMinimum

• `Optional` **exclusiveMinimum**: `number` \| `boolean`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[exclusiveMinimum](codearts_plugin_.workspace.JSONSchema.md#exclusiveminimum)

#### Defined in

[index.d.ts:12877](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12877)

___

### format

• `Optional` **format**: `string`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[format](codearts_plugin_.workspace.JSONSchema.md#format)

#### Defined in

[index.d.ts:12891](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12891)

___

### id

• `Optional` **id**: `string`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[id](codearts_plugin_.workspace.JSONSchema.md#id)

#### Defined in

[index.d.ts:12797](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12797)

___

### if

• `Optional` **if**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[if](codearts_plugin_.workspace.JSONSchema.md#if)

#### Defined in

[index.d.ts:12897](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12897)

___

### ignoreSync

• `Optional` **ignoreSync**: `boolean`

When enabled this setting is ignored during sync and user can override this.

#### Defined in

[index.d.ts:12760](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12760)

___

### included

• `Optional` **included**: `boolean`

When `false` this property is excluded from the registry. Default is to include.

#### Defined in

[index.d.ts:12748](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12748)

___

### items

• `Optional` **items**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md) \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[items](codearts_plugin_.workspace.JSONSchema.md#items)

#### Defined in

[index.d.ts:12839](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12839)

___

### markdownDeprecationMessage

• `Optional` **markdownDeprecationMessage**: `string`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[markdownDeprecationMessage](codearts_plugin_.workspace.JSONSchema.md#markdowndeprecationmessage)

#### Defined in

[index.d.ts:12923](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12923)

___

### markdownDescription

• `Optional` **markdownDescription**: `string`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[markdownDescription](codearts_plugin_.workspace.JSONSchema.md#markdowndescription)

#### Defined in

[index.d.ts:12926](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12926)

___

### markdownEnumDescriptions

• `Optional` **markdownEnumDescriptions**: `string`[]

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[markdownEnumDescriptions](codearts_plugin_.workspace.JSONSchema.md#markdownenumdescriptions)

#### Defined in

[index.d.ts:12925](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12925)

___

### maxContains

• `Optional` **maxContains**: `number`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[maxContains](codearts_plugin_.workspace.JSONSchema.md#maxcontains)

#### Defined in

[index.d.ts:12903](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12903)

___

### maxItems

• `Optional` **maxItems**: `number`

For restricting array max length.

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[maxItems](codearts_plugin_.workspace.JSONSchema.md#maxitems)

#### Defined in

[index.d.ts:12849](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12849)

___

### maxLength

• `Optional` **maxLength**: `number`

For restricting string max length

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[maxLength](codearts_plugin_.workspace.JSONSchema.md#maxlength)

#### Defined in

[index.d.ts:12866](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12866)

___

### maxProperties

• `Optional` **maxProperties**: `number`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[maxProperties](codearts_plugin_.workspace.JSONSchema.md#maxproperties)

#### Defined in

[index.d.ts:12837](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12837)

___

### maximum

• `Optional` **maximum**: `number`

For restricting numeric max values.

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[maximum](codearts_plugin_.workspace.JSONSchema.md#maximum)

#### Defined in

[index.d.ts:12876](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12876)

___

### minContains

• `Optional` **minContains**: `number`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[minContains](codearts_plugin_.workspace.JSONSchema.md#mincontains)

#### Defined in

[index.d.ts:12902](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12902)

___

### minItems

• `Optional` **minItems**: `number`

For restricting array min length.

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[minItems](codearts_plugin_.workspace.JSONSchema.md#minitems)

#### Defined in

[index.d.ts:12844](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12844)

___

### minLength

• `Optional` **minLength**: `number`

For restricting string min length

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[minLength](codearts_plugin_.workspace.JSONSchema.md#minlength)

#### Defined in

[index.d.ts:12861](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12861)

___

### minProperties

• `Optional` **minProperties**: `number`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[minProperties](codearts_plugin_.workspace.JSONSchema.md#minproperties)

#### Defined in

[index.d.ts:12836](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12836)

___

### minimum

• `Optional` **minimum**: `number`

For restricting numeric min values.

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[minimum](codearts_plugin_.workspace.JSONSchema.md#minimum)

#### Defined in

[index.d.ts:12871](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12871)

___

### multipleOf

• `Optional` **multipleOf**: `number`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[multipleOf](codearts_plugin_.workspace.JSONSchema.md#multipleof)

#### Defined in

[index.d.ts:12879](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12879)

___

### not

• `Optional` **not**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[not](codearts_plugin_.workspace.JSONSchema.md#not)

#### Defined in

[index.d.ts:12885](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12885)

___

### oneOf

• `Optional` **oneOf**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[oneOf](codearts_plugin_.workspace.JSONSchema.md#oneof)

#### Defined in

[index.d.ts:12884](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12884)

___

### order

• `Optional` **order**: `number`

When specified, gives an order number for the setting
within the settings editor. Otherwise, the setting is placed at the end.

#### Defined in

[index.d.ts:12782](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12782)

___

### pattern

• `Optional` **pattern**: `string`

For restricting strings to a given regular expression.

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[pattern](codearts_plugin_.workspace.JSONSchema.md#pattern)

#### Defined in

[index.d.ts:12856](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12856)

___

### patternErrorMessage

• `Optional` **patternErrorMessage**: `string`

For giving a tailored error message when a pattern does not match.

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[patternErrorMessage](codearts_plugin_.workspace.JSONSchema.md#patternerrormessage)

#### Defined in

[index.d.ts:12921](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12921)

___

### patternProperties

• `Optional` **patternProperties**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md)

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[patternProperties](codearts_plugin_.workspace.JSONSchema.md#patternproperties)

#### Defined in

[index.d.ts:12828](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12828)

___

### policy

• `Optional` **policy**: [`Policy`](codearts_plugin_.workspace.Policy.md)

When specified, this setting's value can always be overwritten by
a system-wide policy.

#### Defined in

[index.d.ts:12788](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12788)

___

### prefixItems

• `Optional` **prefixItems**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[prefixItems](codearts_plugin_.workspace.JSONSchema.md#prefixitems)

#### Defined in

[index.d.ts:12912](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12912)

___

### properties

• `Optional` **properties**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md)

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[properties](codearts_plugin_.workspace.JSONSchema.md#properties)

#### Defined in

[index.d.ts:12827](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12827)

___

### propertyNames

• `Optional` **propertyNames**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[propertyNames](codearts_plugin_.workspace.JSONSchema.md#propertynames)

#### Defined in

[index.d.ts:12894](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12894)

___

### required

• `Optional` **required**: `string`[]

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[required](codearts_plugin_.workspace.JSONSchema.md#required)

#### Defined in

[index.d.ts:12880](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12880)

___

### restricted

• `Optional` **restricted**: `boolean`

When restricted, value of this configuration will be read only from trusted sources.
For eg., If the workspace is not trusted, then the value of this configuration is not read from workspace settings file.

#### Defined in

[index.d.ts:12743](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12743)

___

### scope

• `Optional` **scope**: [`ConfigurationScope`](../modules/_codearts_plugin_.md#configurationscope)

Configuration scopes determine when a setting is available to the user through the Settings editor and whether the setting is applicable.
If no scope is declared, the default is window.

#### Defined in

[index.d.ts:12737](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12737)

___

### subTitle

• `Optional` **subTitle**: `string`

Subtitle, which can be used as a secondary tree title

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[subTitle](codearts_plugin_.workspace.JSONSchema.md#subtitle)

#### Defined in

[index.d.ts:12935](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12935)

___

### suggestSortText

• `Optional` **suggestSortText**: `string`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[suggestSortText](codearts_plugin_.workspace.JSONSchema.md#suggestsorttext)

#### Defined in

[index.d.ts:12928](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12928)

___

### tags

• `Optional` **tags**: `string`[]

List of tags associated to the property.
 - A tag can be used for filtering
 - Use `experimental` tag for marking the setting as experimental. **Note:** Defaults of experimental settings can be changed by the running experiments.

#### Defined in

[index.d.ts:12755](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12755)

___

### then

• `Optional` **then**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[then](codearts_plugin_.workspace.JSONSchema.md#then)

#### Defined in

[index.d.ts:12898](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12898)

___

### title

• `Optional` **title**: `string`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[title](codearts_plugin_.workspace.JSONSchema.md#title)

#### Defined in

[index.d.ts:12813](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12813)

___

### type

• `Optional` **type**: [`JSONSchemaType`](../modules/codearts_plugin_.workspace.md#jsonschematype) \| [`JSONSchemaType`](../modules/codearts_plugin_.workspace.md#jsonschematype)[]

[`type`](codearts_plugin_.workspace.ConfigurationPropertySchema.md#type) The value of type is dynamically displayed in Settings based on the transferred value.
When type is set to string or number, the input box of the corresponding type is generated on the Settings page.
When type is set to boolean, a checkbox is generated on the settings page.
JSONSchemaType.array Some object and array type settings will be rendered in the settings UI. Simple arrays of number, string, or boolean will be rendered as editable lists.
JSONSchemaType.object Objects that have properties of type string, number, integer, and/or boolean will be rendered as editable grids of keys and values.
Object settings should also have additionalProperties set to either false, or an object with an appropriate type property, to render in the UI.
If an object or array type setting can also contain other types like nested objects, arrays, or null,
then the value won't be rendered in the settings UI and can only be modified by editing the JSON directly.
Users will see a link to Edit in settings.json

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[type](codearts_plugin_.workspace.JSONSchema.md#type)

#### Defined in

[index.d.ts:12812](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12812)

___

### unevaluatedItems

• `Optional` **unevaluatedItems**: `boolean` \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[unevaluatedItems](codearts_plugin_.workspace.JSONSchema.md#unevaluateditems)

#### Defined in

[index.d.ts:12901](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12901)

___

### unevaluatedProperties

• `Optional` **unevaluatedProperties**: `boolean` \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[unevaluatedProperties](codearts_plugin_.workspace.JSONSchema.md#unevaluatedproperties)

#### Defined in

[index.d.ts:12900](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12900)

___

### uniqueItems

• `Optional` **uniqueItems**: `boolean`

#### Inherited from

[JSONSchema](codearts_plugin_.workspace.JSONSchema.md).[uniqueItems](codearts_plugin_.workspace.JSONSchema.md#uniqueitems)

#### Defined in

[index.d.ts:12850](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12850)
