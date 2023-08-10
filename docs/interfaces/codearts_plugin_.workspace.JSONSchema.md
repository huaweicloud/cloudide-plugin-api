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

[index.d.ts:13040](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13040)

___

### $comment

• `Optional` **$comment**: `string`

#### Defined in

[index.d.ts:13028](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13028)

___

### $defs

• `Optional` **$defs**: `Object`

#### Index signature

▪ [name: `string`]: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:13039](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13039)

___

### $dynamicAnchor

• `Optional` **$dynamicAnchor**: `string`

#### Defined in

[index.d.ts:13046](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13046)

___

### $dynamicRef

• `Optional` **$dynamicRef**: `string`

#### Defined in

[index.d.ts:13045](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13045)

___

### $id

• `Optional` **$id**: `string`

#### Defined in

[index.d.ts:12930](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12930)

___

### $recursiveAnchor

• `Optional` **$recursiveAnchor**: `string`

#### Defined in

[index.d.ts:13042](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13042)

___

### $recursiveRef

• `Optional` **$recursiveRef**: `string`

#### Defined in

[index.d.ts:13041](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13041)

___

### $ref

• `Optional` **$ref**: `string`

#### Defined in

[index.d.ts:13013](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13013)

___

### $schema

• `Optional` **$schema**: `string`

#### Defined in

[index.d.ts:12931](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12931)

___

### $vocabulary

• `Optional` **$vocabulary**: `any`

#### Defined in

[index.d.ts:13043](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13043)

___

### additionalItems

• `Optional` **additionalItems**: `boolean` \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12983](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12983)

___

### additionalProperties

• `Optional` **additionalProperties**: `boolean` \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

[`additionalProperties`](codearts_plugin_.workspace.JSONSchema.md#additionalproperties)ConfigurationType
Either a schema or a boolean. If a schema, then used to validate all properties not matched by 'properties' or 'patternProperties'.
If false, then any properties not matched by either will cause this schema to fail.

#### Defined in

[index.d.ts:12967](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12967)

___

### allOf

• `Optional` **allOf**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Defined in

[index.d.ts:13015](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13015)

___

### allowComments

• `Optional` **allowComments**: `boolean`

#### Defined in

[index.d.ts:13061](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13061)

___

### allowTrailingCommas

• `Optional` **allowTrailingCommas**: `boolean`

#### Defined in

[index.d.ts:13062](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13062)

___

### anyOf

• `Optional` **anyOf**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Defined in

[index.d.ts:13014](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13014)

___

### const

• `Optional` **const**: `any`

#### Defined in

[index.d.ts:13024](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13024)

___

### contains

• `Optional` **contains**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:13025](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13025)

___

### default

• `Optional` **default**: `any`

For defining the default value of a property.

#### Defined in

[index.d.ts:12950](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12950)

___

### defaultSnippets

• `Optional` **defaultSnippets**: [`JSONSchemaSnippet`](codearts_plugin_.workspace.JSONSchemaSnippet.md)[]

#### Defined in

[index.d.ts:13047](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13047)

___

### definitions

• `Optional` **definitions**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md)

#### Defined in

[index.d.ts:12951](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12951)

___

### dependencies

• `Optional` **dependencies**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md) \| { `[prop: string]`: `string`[];  }

#### Defined in

[index.d.ts:12970](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12970)

___

### dependentRequired

• `Optional` **dependentRequired**: `Object`

#### Index signature

▪ [prop: `string`]: `string`[]

#### Defined in

[index.d.ts:13037](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13037)

___

### dependentSchemas

• `Optional` **dependentSchemas**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md)

#### Defined in

[index.d.ts:13038](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13038)

___

### deprecated

• `Optional` **deprecated**: `boolean`

#### Defined in

[index.d.ts:13036](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13036)

___

### deprecationMessage

• `Optional` **deprecationMessage**: `string`

#### Defined in

[index.d.ts:13054](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13054)

___

### description

• `Optional` **description**: `string`

Your description appears after the title and before the input field,
except for booleans, where the description is used as the label for the checkbox.
For markdownDescription, in order to add newlines or multiple paragraphs, use the string \n\n to separate the paragraphs instead of just \n.

#### Defined in

[index.d.ts:12958](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12958)

___

### doNotSuggest

• `Optional` **doNotSuggest**: `boolean`

#### Defined in

[index.d.ts:13059](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13059)

___

### else

• `Optional` **else**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:13031](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13031)

___

### enum

• `Optional` **enum**: `any`[]

If you provide an array of items under the enum property, the settings UI will render a dropdown menu.

#### Defined in

[index.d.ts:13022](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13022)

___

### enumDescriptions

• `Optional` **enumDescriptions**: `string`[]

#### Defined in

[index.d.ts:13056](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13056)

___

### errorMessage

• `Optional` **errorMessage**: `string`

#### Defined in

[index.d.ts:13048](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13048)

___

### examples

• `Optional` **examples**: `any`[]

#### Defined in

[index.d.ts:13027](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13027)

___

### exclusiveMaximum

• `Optional` **exclusiveMaximum**: `number` \| `boolean`

#### Defined in

[index.d.ts:13010](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13010)

___

### exclusiveMinimum

• `Optional` **exclusiveMinimum**: `number` \| `boolean`

#### Defined in

[index.d.ts:13009](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13009)

___

### format

• `Optional` **format**: `string`

#### Defined in

[index.d.ts:13023](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13023)

___

### id

• `Optional` **id**: `string`

#### Defined in

[index.d.ts:12929](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12929)

___

### if

• `Optional` **if**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:13029](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13029)

___

### items

• `Optional` **items**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md) \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Defined in

[index.d.ts:12971](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12971)

___

### markdownDeprecationMessage

• `Optional` **markdownDeprecationMessage**: `string`

#### Defined in

[index.d.ts:13055](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13055)

___

### markdownDescription

• `Optional` **markdownDescription**: `string`

#### Defined in

[index.d.ts:13058](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13058)

___

### markdownEnumDescriptions

• `Optional` **markdownEnumDescriptions**: `string`[]

#### Defined in

[index.d.ts:13057](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13057)

___

### maxContains

• `Optional` **maxContains**: `number`

#### Defined in

[index.d.ts:13035](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13035)

___

### maxItems

• `Optional` **maxItems**: `number`

For restricting array max length.

#### Defined in

[index.d.ts:12981](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12981)

___

### maxLength

• `Optional` **maxLength**: `number`

For restricting string max length

#### Defined in

[index.d.ts:12998](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12998)

___

### maxProperties

• `Optional` **maxProperties**: `number`

#### Defined in

[index.d.ts:12969](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12969)

___

### maximum

• `Optional` **maximum**: `number`

For restricting numeric max values.

#### Defined in

[index.d.ts:13008](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13008)

___

### minContains

• `Optional` **minContains**: `number`

#### Defined in

[index.d.ts:13034](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13034)

___

### minItems

• `Optional` **minItems**: `number`

For restricting array min length.

#### Defined in

[index.d.ts:12976](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12976)

___

### minLength

• `Optional` **minLength**: `number`

For restricting string min length

#### Defined in

[index.d.ts:12993](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12993)

___

### minProperties

• `Optional` **minProperties**: `number`

#### Defined in

[index.d.ts:12968](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12968)

___

### minimum

• `Optional` **minimum**: `number`

For restricting numeric min values.

#### Defined in

[index.d.ts:13003](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13003)

___

### multipleOf

• `Optional` **multipleOf**: `number`

#### Defined in

[index.d.ts:13011](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13011)

___

### not

• `Optional` **not**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:13017](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13017)

___

### oneOf

• `Optional` **oneOf**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Defined in

[index.d.ts:13016](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13016)

___

### pattern

• `Optional` **pattern**: `string`

For restricting strings to a given regular expression.

#### Defined in

[index.d.ts:12988](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12988)

___

### patternErrorMessage

• `Optional` **patternErrorMessage**: `string`

For giving a tailored error message when a pattern does not match.

#### Defined in

[index.d.ts:13053](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13053)

___

### patternProperties

• `Optional` **patternProperties**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md)

#### Defined in

[index.d.ts:12960](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12960)

___

### prefixItems

• `Optional` **prefixItems**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Defined in

[index.d.ts:13044](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13044)

___

### properties

• `Optional` **properties**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md)

#### Defined in

[index.d.ts:12959](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12959)

___

### propertyNames

• `Optional` **propertyNames**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:13026](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13026)

___

### required

• `Optional` **required**: `string`[]

#### Defined in

[index.d.ts:13012](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13012)

___

### subTitle

• `Optional` **subTitle**: `string`

Subtitle, which can be used as a secondary tree title

#### Defined in

[index.d.ts:13067](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13067)

___

### suggestSortText

• `Optional` **suggestSortText**: `string`

#### Defined in

[index.d.ts:13060](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13060)

___

### then

• `Optional` **then**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:13030](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13030)

___

### title

• `Optional` **title**: `string`

#### Defined in

[index.d.ts:12945](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12945)

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

[index.d.ts:12944](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12944)

___

### unevaluatedItems

• `Optional` **unevaluatedItems**: `boolean` \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:13033](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13033)

___

### unevaluatedProperties

• `Optional` **unevaluatedProperties**: `boolean` \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:13032](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13032)

___

### uniqueItems

• `Optional` **uniqueItems**: `boolean`

#### Defined in

[index.d.ts:12982](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L12982)
