[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / [workspace](../modules/codearts_plugin_.workspace.md) / JSONSchema

# Interface: JSONSchema

["@codearts/plugin"](../modules/_codearts_plugin_.md).[workspace](../modules/codearts_plugin_.workspace.md).JSONSchema

## Hierarchy

- **`JSONSchema`**

  ↳ [`ConfigurationPropertySchema`](codearts_plugin_.workspace.ConfigurationPropertySchema.md)

## Table of contents

### Properties

- [$anchor](codearts_plugin_.workspace.JSONSchema.md#$anchor)
- [$comment](codearts_plugin_.workspace.JSONSchema.md#$comment)
- [$defs](codearts_plugin_.workspace.JSONSchema.md#$defs)
- [$dynamicAnchor](codearts_plugin_.workspace.JSONSchema.md#$dynamicanchor)
- [$dynamicRef](codearts_plugin_.workspace.JSONSchema.md#$dynamicref)
- [$id](codearts_plugin_.workspace.JSONSchema.md#$id)
- [$recursiveAnchor](codearts_plugin_.workspace.JSONSchema.md#$recursiveanchor)
- [$recursiveRef](codearts_plugin_.workspace.JSONSchema.md#$recursiveref)
- [$ref](codearts_plugin_.workspace.JSONSchema.md#$ref)
- [$schema](codearts_plugin_.workspace.JSONSchema.md#$schema)
- [$vocabulary](codearts_plugin_.workspace.JSONSchema.md#$vocabulary)
- [additionalItems](codearts_plugin_.workspace.JSONSchema.md#additionalitems)
- [additionalProperties](codearts_plugin_.workspace.JSONSchema.md#additionalproperties)
- [allOf](codearts_plugin_.workspace.JSONSchema.md#allof)
- [allowComments](codearts_plugin_.workspace.JSONSchema.md#allowcomments)
- [allowTrailingCommas](codearts_plugin_.workspace.JSONSchema.md#allowtrailingcommas)
- [anyOf](codearts_plugin_.workspace.JSONSchema.md#anyof)
- [const](codearts_plugin_.workspace.JSONSchema.md#const)
- [contains](codearts_plugin_.workspace.JSONSchema.md#contains)
- [default](codearts_plugin_.workspace.JSONSchema.md#default)
- [defaultSnippets](codearts_plugin_.workspace.JSONSchema.md#defaultsnippets)
- [definitions](codearts_plugin_.workspace.JSONSchema.md#definitions)
- [dependencies](codearts_plugin_.workspace.JSONSchema.md#dependencies)
- [dependentRequired](codearts_plugin_.workspace.JSONSchema.md#dependentrequired)
- [dependentSchemas](codearts_plugin_.workspace.JSONSchema.md#dependentschemas)
- [deprecated](codearts_plugin_.workspace.JSONSchema.md#deprecated)
- [deprecationMessage](codearts_plugin_.workspace.JSONSchema.md#deprecationmessage)
- [description](codearts_plugin_.workspace.JSONSchema.md#description)
- [doNotSuggest](codearts_plugin_.workspace.JSONSchema.md#donotsuggest)
- [else](codearts_plugin_.workspace.JSONSchema.md#else)
- [enum](codearts_plugin_.workspace.JSONSchema.md#enum)
- [enumDescriptions](codearts_plugin_.workspace.JSONSchema.md#enumdescriptions)
- [errorMessage](codearts_plugin_.workspace.JSONSchema.md#errormessage)
- [examples](codearts_plugin_.workspace.JSONSchema.md#examples)
- [exclusiveMaximum](codearts_plugin_.workspace.JSONSchema.md#exclusivemaximum)
- [exclusiveMinimum](codearts_plugin_.workspace.JSONSchema.md#exclusiveminimum)
- [format](codearts_plugin_.workspace.JSONSchema.md#format)
- [id](codearts_plugin_.workspace.JSONSchema.md#id)
- [if](codearts_plugin_.workspace.JSONSchema.md#if)
- [items](codearts_plugin_.workspace.JSONSchema.md#items)
- [markdownDeprecationMessage](codearts_plugin_.workspace.JSONSchema.md#markdowndeprecationmessage)
- [markdownDescription](codearts_plugin_.workspace.JSONSchema.md#markdowndescription)
- [markdownEnumDescriptions](codearts_plugin_.workspace.JSONSchema.md#markdownenumdescriptions)
- [maxContains](codearts_plugin_.workspace.JSONSchema.md#maxcontains)
- [maxItems](codearts_plugin_.workspace.JSONSchema.md#maxitems)
- [maxLength](codearts_plugin_.workspace.JSONSchema.md#maxlength)
- [maxProperties](codearts_plugin_.workspace.JSONSchema.md#maxproperties)
- [maximum](codearts_plugin_.workspace.JSONSchema.md#maximum)
- [minContains](codearts_plugin_.workspace.JSONSchema.md#mincontains)
- [minItems](codearts_plugin_.workspace.JSONSchema.md#minitems)
- [minLength](codearts_plugin_.workspace.JSONSchema.md#minlength)
- [minProperties](codearts_plugin_.workspace.JSONSchema.md#minproperties)
- [minimum](codearts_plugin_.workspace.JSONSchema.md#minimum)
- [multipleOf](codearts_plugin_.workspace.JSONSchema.md#multipleof)
- [not](codearts_plugin_.workspace.JSONSchema.md#not)
- [oneOf](codearts_plugin_.workspace.JSONSchema.md#oneof)
- [pattern](codearts_plugin_.workspace.JSONSchema.md#pattern)
- [patternErrorMessage](codearts_plugin_.workspace.JSONSchema.md#patternerrormessage)
- [patternProperties](codearts_plugin_.workspace.JSONSchema.md#patternproperties)
- [prefixItems](codearts_plugin_.workspace.JSONSchema.md#prefixitems)
- [properties](codearts_plugin_.workspace.JSONSchema.md#properties)
- [propertyNames](codearts_plugin_.workspace.JSONSchema.md#propertynames)
- [required](codearts_plugin_.workspace.JSONSchema.md#required)
- [subTitle](codearts_plugin_.workspace.JSONSchema.md#subtitle)
- [suggestSortText](codearts_plugin_.workspace.JSONSchema.md#suggestsorttext)
- [then](codearts_plugin_.workspace.JSONSchema.md#then)
- [title](codearts_plugin_.workspace.JSONSchema.md#title)
- [type](codearts_plugin_.workspace.JSONSchema.md#type)
- [unevaluatedItems](codearts_plugin_.workspace.JSONSchema.md#unevaluateditems)
- [unevaluatedProperties](codearts_plugin_.workspace.JSONSchema.md#unevaluatedproperties)
- [uniqueItems](codearts_plugin_.workspace.JSONSchema.md#uniqueitems)

## Properties

### $anchor

• `Optional` **$anchor**: `string`

#### Defined in

[index.d.ts:12856](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12856)

___

### $comment

• `Optional` **$comment**: `string`

#### Defined in

[index.d.ts:12844](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12844)

___

### $defs

• `Optional` **$defs**: `Object`

#### Index signature

▪ [name: `string`]: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12855](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12855)

___

### $dynamicAnchor

• `Optional` **$dynamicAnchor**: `string`

#### Defined in

[index.d.ts:12862](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12862)

___

### $dynamicRef

• `Optional` **$dynamicRef**: `string`

#### Defined in

[index.d.ts:12861](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12861)

___

### $id

• `Optional` **$id**: `string`

#### Defined in

[index.d.ts:12746](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12746)

___

### $recursiveAnchor

• `Optional` **$recursiveAnchor**: `string`

#### Defined in

[index.d.ts:12858](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12858)

___

### $recursiveRef

• `Optional` **$recursiveRef**: `string`

#### Defined in

[index.d.ts:12857](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12857)

___

### $ref

• `Optional` **$ref**: `string`

#### Defined in

[index.d.ts:12829](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12829)

___

### $schema

• `Optional` **$schema**: `string`

#### Defined in

[index.d.ts:12747](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12747)

___

### $vocabulary

• `Optional` **$vocabulary**: `any`

#### Defined in

[index.d.ts:12859](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12859)

___

### additionalItems

• `Optional` **additionalItems**: `boolean` \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12799](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12799)

___

### additionalProperties

• `Optional` **additionalProperties**: `boolean` \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

[`additionalProperties`](codearts_plugin_.workspace.JSONSchema.md#additionalproperties)ConfigurationType
Either a schema or a boolean. If a schema, then used to validate all properties not matched by 'properties' or 'patternProperties'.
If false, then any properties not matched by either will cause this schema to fail.

#### Defined in

[index.d.ts:12783](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12783)

___

### allOf

• `Optional` **allOf**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Defined in

[index.d.ts:12831](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12831)

___

### allowComments

• `Optional` **allowComments**: `boolean`

#### Defined in

[index.d.ts:12877](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12877)

___

### allowTrailingCommas

• `Optional` **allowTrailingCommas**: `boolean`

#### Defined in

[index.d.ts:12878](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12878)

___

### anyOf

• `Optional` **anyOf**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Defined in

[index.d.ts:12830](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12830)

___

### const

• `Optional` **const**: `any`

#### Defined in

[index.d.ts:12840](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12840)

___

### contains

• `Optional` **contains**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12841](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12841)

___

### default

• `Optional` **default**: `any`

For defining the default value of a property.

#### Defined in

[index.d.ts:12766](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12766)

___

### defaultSnippets

• `Optional` **defaultSnippets**: [`JSONSchemaSnippet`](codearts_plugin_.workspace.JSONSchemaSnippet.md)[]

#### Defined in

[index.d.ts:12863](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12863)

___

### definitions

• `Optional` **definitions**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md)

#### Defined in

[index.d.ts:12767](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12767)

___

### dependencies

• `Optional` **dependencies**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md) \| { `[prop: string]`: `string`[];  }

#### Defined in

[index.d.ts:12786](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12786)

___

### dependentRequired

• `Optional` **dependentRequired**: `Object`

#### Index signature

▪ [prop: `string`]: `string`[]

#### Defined in

[index.d.ts:12853](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12853)

___

### dependentSchemas

• `Optional` **dependentSchemas**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md)

#### Defined in

[index.d.ts:12854](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12854)

___

### deprecated

• `Optional` **deprecated**: `boolean`

#### Defined in

[index.d.ts:12852](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12852)

___

### deprecationMessage

• `Optional` **deprecationMessage**: `string`

#### Defined in

[index.d.ts:12870](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12870)

___

### description

• `Optional` **description**: `string`

Your description appears after the title and before the input field,
except for booleans, where the description is used as the label for the checkbox.
For markdownDescription, in order to add newlines or multiple paragraphs, use the string \n\n to separate the paragraphs instead of just \n.

#### Defined in

[index.d.ts:12774](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12774)

___

### doNotSuggest

• `Optional` **doNotSuggest**: `boolean`

#### Defined in

[index.d.ts:12875](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12875)

___

### else

• `Optional` **else**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12847](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12847)

___

### enum

• `Optional` **enum**: `any`[]

If you provide an array of items under the enum property, the settings UI will render a dropdown menu.

#### Defined in

[index.d.ts:12838](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12838)

___

### enumDescriptions

• `Optional` **enumDescriptions**: `string`[]

#### Defined in

[index.d.ts:12872](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12872)

___

### errorMessage

• `Optional` **errorMessage**: `string`

#### Defined in

[index.d.ts:12864](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12864)

___

### examples

• `Optional` **examples**: `any`[]

#### Defined in

[index.d.ts:12843](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12843)

___

### exclusiveMaximum

• `Optional` **exclusiveMaximum**: `number` \| `boolean`

#### Defined in

[index.d.ts:12826](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12826)

___

### exclusiveMinimum

• `Optional` **exclusiveMinimum**: `number` \| `boolean`

#### Defined in

[index.d.ts:12825](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12825)

___

### format

• `Optional` **format**: `string`

#### Defined in

[index.d.ts:12839](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12839)

___

### id

• `Optional` **id**: `string`

#### Defined in

[index.d.ts:12745](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12745)

___

### if

• `Optional` **if**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12845](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12845)

___

### items

• `Optional` **items**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md) \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Defined in

[index.d.ts:12787](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12787)

___

### markdownDeprecationMessage

• `Optional` **markdownDeprecationMessage**: `string`

#### Defined in

[index.d.ts:12871](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12871)

___

### markdownDescription

• `Optional` **markdownDescription**: `string`

#### Defined in

[index.d.ts:12874](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12874)

___

### markdownEnumDescriptions

• `Optional` **markdownEnumDescriptions**: `string`[]

#### Defined in

[index.d.ts:12873](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12873)

___

### maxContains

• `Optional` **maxContains**: `number`

#### Defined in

[index.d.ts:12851](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12851)

___

### maxItems

• `Optional` **maxItems**: `number`

For restricting array max length.

#### Defined in

[index.d.ts:12797](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12797)

___

### maxLength

• `Optional` **maxLength**: `number`

For restricting string max length

#### Defined in

[index.d.ts:12814](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12814)

___

### maxProperties

• `Optional` **maxProperties**: `number`

#### Defined in

[index.d.ts:12785](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12785)

___

### maximum

• `Optional` **maximum**: `number`

For restricting numeric max values.

#### Defined in

[index.d.ts:12824](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12824)

___

### minContains

• `Optional` **minContains**: `number`

#### Defined in

[index.d.ts:12850](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12850)

___

### minItems

• `Optional` **minItems**: `number`

For restricting array min length.

#### Defined in

[index.d.ts:12792](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12792)

___

### minLength

• `Optional` **minLength**: `number`

For restricting string min length

#### Defined in

[index.d.ts:12809](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12809)

___

### minProperties

• `Optional` **minProperties**: `number`

#### Defined in

[index.d.ts:12784](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12784)

___

### minimum

• `Optional` **minimum**: `number`

For restricting numeric min values.

#### Defined in

[index.d.ts:12819](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12819)

___

### multipleOf

• `Optional` **multipleOf**: `number`

#### Defined in

[index.d.ts:12827](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12827)

___

### not

• `Optional` **not**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12833](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12833)

___

### oneOf

• `Optional` **oneOf**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Defined in

[index.d.ts:12832](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12832)

___

### pattern

• `Optional` **pattern**: `string`

For restricting strings to a given regular expression.

#### Defined in

[index.d.ts:12804](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12804)

___

### patternErrorMessage

• `Optional` **patternErrorMessage**: `string`

For giving a tailored error message when a pattern does not match.

#### Defined in

[index.d.ts:12869](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12869)

___

### patternProperties

• `Optional` **patternProperties**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md)

#### Defined in

[index.d.ts:12776](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12776)

___

### prefixItems

• `Optional` **prefixItems**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Defined in

[index.d.ts:12860](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12860)

___

### properties

• `Optional` **properties**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md)

#### Defined in

[index.d.ts:12775](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12775)

___

### propertyNames

• `Optional` **propertyNames**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12842](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12842)

___

### required

• `Optional` **required**: `string`[]

#### Defined in

[index.d.ts:12828](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12828)

___

### subTitle

• `Optional` **subTitle**: `string`

Subtitle, which can be used as a secondary tree title

#### Defined in

[index.d.ts:12883](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12883)

___

### suggestSortText

• `Optional` **suggestSortText**: `string`

#### Defined in

[index.d.ts:12876](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12876)

___

### then

• `Optional` **then**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12846](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12846)

___

### title

• `Optional` **title**: `string`

#### Defined in

[index.d.ts:12761](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12761)

___

### type

• `Optional` **type**: [`JSONSchemaType`](../modules/codearts_plugin_.workspace.md#jsonschematype) \| [`JSONSchemaType`](../modules/codearts_plugin_.workspace.md#jsonschematype)[]

[`type`](codearts_plugin_.workspace.JSONSchema.md#type) The value of type is dynamically displayed in Settings based on the transferred value.
When type is set to string or number, the input box of the corresponding type is generated on the Settings page.
When type is set to boolean, a checkbox is generated on the settings page.
JSONSchemaType.array Some object and array type settings will be rendered in the settings UI. Simple arrays of number, string, or boolean will be rendered as editable lists.
JSONSchemaType.object Objects that have properties of type string, number, integer, and/or boolean will be rendered as editable grids of keys and values.
Object settings should also have additionalProperties set to either false, or an object with an appropriate type property, to render in the UI.
If an object or array type setting can also contain other types like nested objects, arrays, or null,
then the value won't be rendered in the settings UI and can only be modified by editing the JSON directly.
Users will see a link to Edit in settings.json

#### Defined in

[index.d.ts:12760](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12760)

___

### unevaluatedItems

• `Optional` **unevaluatedItems**: `boolean` \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12849](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12849)

___

### unevaluatedProperties

• `Optional` **unevaluatedProperties**: `boolean` \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12848](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12848)

___

### uniqueItems

• `Optional` **uniqueItems**: `boolean`

#### Defined in

[index.d.ts:12798](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L12798)
