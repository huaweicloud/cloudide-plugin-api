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

[index.d.ts:12908](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12908)

___

### $comment

• `Optional` **$comment**: `string`

#### Defined in

[index.d.ts:12896](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12896)

___

### $defs

• `Optional` **$defs**: `Object`

#### Index signature

▪ [name: `string`]: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12907](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12907)

___

### $dynamicAnchor

• `Optional` **$dynamicAnchor**: `string`

#### Defined in

[index.d.ts:12914](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12914)

___

### $dynamicRef

• `Optional` **$dynamicRef**: `string`

#### Defined in

[index.d.ts:12913](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12913)

___

### $id

• `Optional` **$id**: `string`

#### Defined in

[index.d.ts:12798](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12798)

___

### $recursiveAnchor

• `Optional` **$recursiveAnchor**: `string`

#### Defined in

[index.d.ts:12910](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12910)

___

### $recursiveRef

• `Optional` **$recursiveRef**: `string`

#### Defined in

[index.d.ts:12909](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12909)

___

### $ref

• `Optional` **$ref**: `string`

#### Defined in

[index.d.ts:12881](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12881)

___

### $schema

• `Optional` **$schema**: `string`

#### Defined in

[index.d.ts:12799](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12799)

___

### $vocabulary

• `Optional` **$vocabulary**: `any`

#### Defined in

[index.d.ts:12911](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12911)

___

### additionalItems

• `Optional` **additionalItems**: `boolean` \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12851](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12851)

___

### additionalProperties

• `Optional` **additionalProperties**: `boolean` \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

[`additionalProperties`](codearts_plugin_.workspace.JSONSchema.md#additionalproperties)ConfigurationType
Either a schema or a boolean. If a schema, then used to validate all properties not matched by 'properties' or 'patternProperties'.
If false, then any properties not matched by either will cause this schema to fail.

#### Defined in

[index.d.ts:12835](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12835)

___

### allOf

• `Optional` **allOf**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Defined in

[index.d.ts:12883](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12883)

___

### allowComments

• `Optional` **allowComments**: `boolean`

#### Defined in

[index.d.ts:12929](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12929)

___

### allowTrailingCommas

• `Optional` **allowTrailingCommas**: `boolean`

#### Defined in

[index.d.ts:12930](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12930)

___

### anyOf

• `Optional` **anyOf**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Defined in

[index.d.ts:12882](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12882)

___

### const

• `Optional` **const**: `any`

#### Defined in

[index.d.ts:12892](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12892)

___

### contains

• `Optional` **contains**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12893](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12893)

___

### default

• `Optional` **default**: `any`

For defining the default value of a property.

#### Defined in

[index.d.ts:12818](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12818)

___

### defaultSnippets

• `Optional` **defaultSnippets**: [`JSONSchemaSnippet`](codearts_plugin_.workspace.JSONSchemaSnippet.md)[]

#### Defined in

[index.d.ts:12915](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12915)

___

### definitions

• `Optional` **definitions**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md)

#### Defined in

[index.d.ts:12819](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12819)

___

### dependencies

• `Optional` **dependencies**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md) \| { `[prop: string]`: `string`[];  }

#### Defined in

[index.d.ts:12838](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12838)

___

### dependentRequired

• `Optional` **dependentRequired**: `Object`

#### Index signature

▪ [prop: `string`]: `string`[]

#### Defined in

[index.d.ts:12905](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12905)

___

### dependentSchemas

• `Optional` **dependentSchemas**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md)

#### Defined in

[index.d.ts:12906](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12906)

___

### deprecated

• `Optional` **deprecated**: `boolean`

#### Defined in

[index.d.ts:12904](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12904)

___

### deprecationMessage

• `Optional` **deprecationMessage**: `string`

#### Defined in

[index.d.ts:12922](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12922)

___

### description

• `Optional` **description**: `string`

Your description appears after the title and before the input field,
except for booleans, where the description is used as the label for the checkbox.
For markdownDescription, in order to add newlines or multiple paragraphs, use the string \n\n to separate the paragraphs instead of just \n.

#### Defined in

[index.d.ts:12826](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12826)

___

### doNotSuggest

• `Optional` **doNotSuggest**: `boolean`

#### Defined in

[index.d.ts:12927](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12927)

___

### else

• `Optional` **else**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12899](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12899)

___

### enum

• `Optional` **enum**: `any`[]

If you provide an array of items under the enum property, the settings UI will render a dropdown menu.

#### Defined in

[index.d.ts:12890](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12890)

___

### enumDescriptions

• `Optional` **enumDescriptions**: `string`[]

#### Defined in

[index.d.ts:12924](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12924)

___

### errorMessage

• `Optional` **errorMessage**: `string`

#### Defined in

[index.d.ts:12916](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12916)

___

### examples

• `Optional` **examples**: `any`[]

#### Defined in

[index.d.ts:12895](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12895)

___

### exclusiveMaximum

• `Optional` **exclusiveMaximum**: `number` \| `boolean`

#### Defined in

[index.d.ts:12878](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12878)

___

### exclusiveMinimum

• `Optional` **exclusiveMinimum**: `number` \| `boolean`

#### Defined in

[index.d.ts:12877](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12877)

___

### format

• `Optional` **format**: `string`

#### Defined in

[index.d.ts:12891](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12891)

___

### id

• `Optional` **id**: `string`

#### Defined in

[index.d.ts:12797](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12797)

___

### if

• `Optional` **if**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12897](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12897)

___

### items

• `Optional` **items**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md) \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Defined in

[index.d.ts:12839](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12839)

___

### markdownDeprecationMessage

• `Optional` **markdownDeprecationMessage**: `string`

#### Defined in

[index.d.ts:12923](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12923)

___

### markdownDescription

• `Optional` **markdownDescription**: `string`

#### Defined in

[index.d.ts:12926](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12926)

___

### markdownEnumDescriptions

• `Optional` **markdownEnumDescriptions**: `string`[]

#### Defined in

[index.d.ts:12925](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12925)

___

### maxContains

• `Optional` **maxContains**: `number`

#### Defined in

[index.d.ts:12903](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12903)

___

### maxItems

• `Optional` **maxItems**: `number`

For restricting array max length.

#### Defined in

[index.d.ts:12849](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12849)

___

### maxLength

• `Optional` **maxLength**: `number`

For restricting string max length

#### Defined in

[index.d.ts:12866](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12866)

___

### maxProperties

• `Optional` **maxProperties**: `number`

#### Defined in

[index.d.ts:12837](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12837)

___

### maximum

• `Optional` **maximum**: `number`

For restricting numeric max values.

#### Defined in

[index.d.ts:12876](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12876)

___

### minContains

• `Optional` **minContains**: `number`

#### Defined in

[index.d.ts:12902](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12902)

___

### minItems

• `Optional` **minItems**: `number`

For restricting array min length.

#### Defined in

[index.d.ts:12844](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12844)

___

### minLength

• `Optional` **minLength**: `number`

For restricting string min length

#### Defined in

[index.d.ts:12861](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12861)

___

### minProperties

• `Optional` **minProperties**: `number`

#### Defined in

[index.d.ts:12836](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12836)

___

### minimum

• `Optional` **minimum**: `number`

For restricting numeric min values.

#### Defined in

[index.d.ts:12871](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12871)

___

### multipleOf

• `Optional` **multipleOf**: `number`

#### Defined in

[index.d.ts:12879](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12879)

___

### not

• `Optional` **not**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12885](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12885)

___

### oneOf

• `Optional` **oneOf**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Defined in

[index.d.ts:12884](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12884)

___

### pattern

• `Optional` **pattern**: `string`

For restricting strings to a given regular expression.

#### Defined in

[index.d.ts:12856](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12856)

___

### patternErrorMessage

• `Optional` **patternErrorMessage**: `string`

For giving a tailored error message when a pattern does not match.

#### Defined in

[index.d.ts:12921](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12921)

___

### patternProperties

• `Optional` **patternProperties**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md)

#### Defined in

[index.d.ts:12828](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12828)

___

### prefixItems

• `Optional` **prefixItems**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Defined in

[index.d.ts:12912](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12912)

___

### properties

• `Optional` **properties**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md)

#### Defined in

[index.d.ts:12827](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12827)

___

### propertyNames

• `Optional` **propertyNames**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12894](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12894)

___

### required

• `Optional` **required**: `string`[]

#### Defined in

[index.d.ts:12880](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12880)

___

### subTitle

• `Optional` **subTitle**: `string`

Subtitle, which can be used as a secondary tree title

#### Defined in

[index.d.ts:12935](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12935)

___

### suggestSortText

• `Optional` **suggestSortText**: `string`

#### Defined in

[index.d.ts:12928](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12928)

___

### then

• `Optional` **then**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12898](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12898)

___

### title

• `Optional` **title**: `string`

#### Defined in

[index.d.ts:12813](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12813)

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

[index.d.ts:12812](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12812)

___

### unevaluatedItems

• `Optional` **unevaluatedItems**: `boolean` \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12901](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12901)

___

### unevaluatedProperties

• `Optional` **unevaluatedProperties**: `boolean` \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12900](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12900)

___

### uniqueItems

• `Optional` **uniqueItems**: `boolean`

#### Defined in

[index.d.ts:12850](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12850)
