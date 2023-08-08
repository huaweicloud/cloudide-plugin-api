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

[index.d.ts:13011](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13011)

___

### $comment

• `Optional` **$comment**: `string`

#### Defined in

[index.d.ts:12999](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12999)

___

### $defs

• `Optional` **$defs**: `Object`

#### Index signature

▪ [name: `string`]: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:13010](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13010)

___

### $dynamicAnchor

• `Optional` **$dynamicAnchor**: `string`

#### Defined in

[index.d.ts:13017](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13017)

___

### $dynamicRef

• `Optional` **$dynamicRef**: `string`

#### Defined in

[index.d.ts:13016](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13016)

___

### $id

• `Optional` **$id**: `string`

#### Defined in

[index.d.ts:12901](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12901)

___

### $recursiveAnchor

• `Optional` **$recursiveAnchor**: `string`

#### Defined in

[index.d.ts:13013](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13013)

___

### $recursiveRef

• `Optional` **$recursiveRef**: `string`

#### Defined in

[index.d.ts:13012](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13012)

___

### $ref

• `Optional` **$ref**: `string`

#### Defined in

[index.d.ts:12984](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12984)

___

### $schema

• `Optional` **$schema**: `string`

#### Defined in

[index.d.ts:12902](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12902)

___

### $vocabulary

• `Optional` **$vocabulary**: `any`

#### Defined in

[index.d.ts:13014](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13014)

___

### additionalItems

• `Optional` **additionalItems**: `boolean` \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12954](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12954)

___

### additionalProperties

• `Optional` **additionalProperties**: `boolean` \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

[`additionalProperties`](codearts_plugin_.workspace.JSONSchema.md#additionalproperties)ConfigurationType
Either a schema or a boolean. If a schema, then used to validate all properties not matched by 'properties' or 'patternProperties'.
If false, then any properties not matched by either will cause this schema to fail.

#### Defined in

[index.d.ts:12938](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12938)

___

### allOf

• `Optional` **allOf**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Defined in

[index.d.ts:12986](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12986)

___

### allowComments

• `Optional` **allowComments**: `boolean`

#### Defined in

[index.d.ts:13032](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13032)

___

### allowTrailingCommas

• `Optional` **allowTrailingCommas**: `boolean`

#### Defined in

[index.d.ts:13033](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13033)

___

### anyOf

• `Optional` **anyOf**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Defined in

[index.d.ts:12985](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12985)

___

### const

• `Optional` **const**: `any`

#### Defined in

[index.d.ts:12995](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12995)

___

### contains

• `Optional` **contains**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12996](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12996)

___

### default

• `Optional` **default**: `any`

For defining the default value of a property.

#### Defined in

[index.d.ts:12921](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12921)

___

### defaultSnippets

• `Optional` **defaultSnippets**: [`JSONSchemaSnippet`](codearts_plugin_.workspace.JSONSchemaSnippet.md)[]

#### Defined in

[index.d.ts:13018](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13018)

___

### definitions

• `Optional` **definitions**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md)

#### Defined in

[index.d.ts:12922](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12922)

___

### dependencies

• `Optional` **dependencies**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md) \| { `[prop: string]`: `string`[];  }

#### Defined in

[index.d.ts:12941](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12941)

___

### dependentRequired

• `Optional` **dependentRequired**: `Object`

#### Index signature

▪ [prop: `string`]: `string`[]

#### Defined in

[index.d.ts:13008](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13008)

___

### dependentSchemas

• `Optional` **dependentSchemas**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md)

#### Defined in

[index.d.ts:13009](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13009)

___

### deprecated

• `Optional` **deprecated**: `boolean`

#### Defined in

[index.d.ts:13007](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13007)

___

### deprecationMessage

• `Optional` **deprecationMessage**: `string`

#### Defined in

[index.d.ts:13025](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13025)

___

### description

• `Optional` **description**: `string`

Your description appears after the title and before the input field,
except for booleans, where the description is used as the label for the checkbox.
For markdownDescription, in order to add newlines or multiple paragraphs, use the string \n\n to separate the paragraphs instead of just \n.

#### Defined in

[index.d.ts:12929](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12929)

___

### doNotSuggest

• `Optional` **doNotSuggest**: `boolean`

#### Defined in

[index.d.ts:13030](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13030)

___

### else

• `Optional` **else**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:13002](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13002)

___

### enum

• `Optional` **enum**: `any`[]

If you provide an array of items under the enum property, the settings UI will render a dropdown menu.

#### Defined in

[index.d.ts:12993](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12993)

___

### enumDescriptions

• `Optional` **enumDescriptions**: `string`[]

#### Defined in

[index.d.ts:13027](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13027)

___

### errorMessage

• `Optional` **errorMessage**: `string`

#### Defined in

[index.d.ts:13019](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13019)

___

### examples

• `Optional` **examples**: `any`[]

#### Defined in

[index.d.ts:12998](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12998)

___

### exclusiveMaximum

• `Optional` **exclusiveMaximum**: `number` \| `boolean`

#### Defined in

[index.d.ts:12981](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12981)

___

### exclusiveMinimum

• `Optional` **exclusiveMinimum**: `number` \| `boolean`

#### Defined in

[index.d.ts:12980](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12980)

___

### format

• `Optional` **format**: `string`

#### Defined in

[index.d.ts:12994](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12994)

___

### id

• `Optional` **id**: `string`

#### Defined in

[index.d.ts:12900](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12900)

___

### if

• `Optional` **if**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:13000](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13000)

___

### items

• `Optional` **items**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md) \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Defined in

[index.d.ts:12942](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12942)

___

### markdownDeprecationMessage

• `Optional` **markdownDeprecationMessage**: `string`

#### Defined in

[index.d.ts:13026](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13026)

___

### markdownDescription

• `Optional` **markdownDescription**: `string`

#### Defined in

[index.d.ts:13029](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13029)

___

### markdownEnumDescriptions

• `Optional` **markdownEnumDescriptions**: `string`[]

#### Defined in

[index.d.ts:13028](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13028)

___

### maxContains

• `Optional` **maxContains**: `number`

#### Defined in

[index.d.ts:13006](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13006)

___

### maxItems

• `Optional` **maxItems**: `number`

For restricting array max length.

#### Defined in

[index.d.ts:12952](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12952)

___

### maxLength

• `Optional` **maxLength**: `number`

For restricting string max length

#### Defined in

[index.d.ts:12969](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12969)

___

### maxProperties

• `Optional` **maxProperties**: `number`

#### Defined in

[index.d.ts:12940](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12940)

___

### maximum

• `Optional` **maximum**: `number`

For restricting numeric max values.

#### Defined in

[index.d.ts:12979](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12979)

___

### minContains

• `Optional` **minContains**: `number`

#### Defined in

[index.d.ts:13005](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13005)

___

### minItems

• `Optional` **minItems**: `number`

For restricting array min length.

#### Defined in

[index.d.ts:12947](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12947)

___

### minLength

• `Optional` **minLength**: `number`

For restricting string min length

#### Defined in

[index.d.ts:12964](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12964)

___

### minProperties

• `Optional` **minProperties**: `number`

#### Defined in

[index.d.ts:12939](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12939)

___

### minimum

• `Optional` **minimum**: `number`

For restricting numeric min values.

#### Defined in

[index.d.ts:12974](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12974)

___

### multipleOf

• `Optional` **multipleOf**: `number`

#### Defined in

[index.d.ts:12982](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12982)

___

### not

• `Optional` **not**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12988](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12988)

___

### oneOf

• `Optional` **oneOf**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Defined in

[index.d.ts:12987](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12987)

___

### pattern

• `Optional` **pattern**: `string`

For restricting strings to a given regular expression.

#### Defined in

[index.d.ts:12959](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12959)

___

### patternErrorMessage

• `Optional` **patternErrorMessage**: `string`

For giving a tailored error message when a pattern does not match.

#### Defined in

[index.d.ts:13024](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13024)

___

### patternProperties

• `Optional` **patternProperties**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md)

#### Defined in

[index.d.ts:12931](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12931)

___

### prefixItems

• `Optional` **prefixItems**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)[]

#### Defined in

[index.d.ts:13015](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13015)

___

### properties

• `Optional` **properties**: [`JSONSchemaMap`](codearts_plugin_.workspace.JSONSchemaMap.md)

#### Defined in

[index.d.ts:12930](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12930)

___

### propertyNames

• `Optional` **propertyNames**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:12997](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12997)

___

### required

• `Optional` **required**: `string`[]

#### Defined in

[index.d.ts:12983](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12983)

___

### subTitle

• `Optional` **subTitle**: `string`

Subtitle, which can be used as a secondary tree title

#### Defined in

[index.d.ts:13038](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13038)

___

### suggestSortText

• `Optional` **suggestSortText**: `string`

#### Defined in

[index.d.ts:13031](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13031)

___

### then

• `Optional` **then**: [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:13001](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13001)

___

### title

• `Optional` **title**: `string`

#### Defined in

[index.d.ts:12916](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12916)

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

[index.d.ts:12915](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12915)

___

### unevaluatedItems

• `Optional` **unevaluatedItems**: `boolean` \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:13004](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13004)

___

### unevaluatedProperties

• `Optional` **unevaluatedProperties**: `boolean` \| [`JSONSchema`](codearts_plugin_.workspace.JSONSchema.md)

#### Defined in

[index.d.ts:13003](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L13003)

___

### uniqueItems

• `Optional` **uniqueItems**: `boolean`

#### Defined in

[index.d.ts:12953](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12953)
