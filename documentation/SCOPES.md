# SCOPES

**NOTE: This is a work-in-progress!**

Different types of symbols and operators have their own "scope", which can be edited to use a different color or font style. A couple of lists can be found [here](https://www.sublimetext.com/docs/3/scope_naming.html#keyword) and [here](https://macromates.com/manual/en/language_grammars), though keep in mind these aren't necessarily exhaustive - there are certain properties that you won't find on either of these lists.

Scopes should be styled based on specificity - the broadest scopes should be styled first, then the more specific items.

## `comment`

- `line`
  - `double-slash`
  - `double-dash`
  - `number-sign`
  - `percentage`
- `block`
  - `documentation`

## `constant`

- `numeric`
  - `integer`
    - `binary`
    - `octal`
    - `decimal`
    - `hexadecimal`
    - `other`
  - `float`
    - `binary`
    - `octal`
    - `decimal`
    - `hexadecimal`
    - `other`
  - `complex`
    - `real`
    - `imaginary`
- `character`
  - `escape`
- `language`
- `character`
  - `escape`
- `other`
  - `placeholder`

## `entity`

- `name`
  - `class`
    - `forward-decl`
  - `enum`
  - `function`
    - `constructor`
    - `destructor`
  - `impl`
  - `interface`
  - `section`
  - `struct`
  - `tag`
  - `trait`
  - `type`
  - `union`
  - `namespace`
  - `constant`
  - `label`
- `other`
  - `inherited-class`
  - `attribute-name`

## `invalid`

- `illegal`
- `deprecated`

## `keyword`

- `control`
  - `conditional`
  - `import`
- `operator`
  - `assignment`
  - `arithmetic`
  - `bitwise`
  - `logical`
  - `word`
- `other`
- `declaration`
  - `function`
  - `class`
  - `struct`
  - `enum`
  - `union`
  - `trait`
  - `interface`
  - `impl`

## `markup`

- `underline`
  - `link`
- `bold`
- `heading`
- `italic`
- `list`
  - `numbered`
  - `unnumbered`
- `quote`
- `raw`
  - `inline`
  - `block`
- `other`
- `inserted`
- `deleted`

## `meta`

- `toc-list`
- `class`
- `struct`
- `enum`
- `union`
- `trait`
- `interface`
- `impl`
- `type`
- `block`
- `braces`
- `group`
- `parens`
- `brackets`
- `function`
  - `parameters`
  - `return-type`
- `function-call`
- `namespace`
- `preprocessor`
- `annotation`
  - `identifier`
  - `parameters`
- `generic`
- `path`
- `string`
- `interpolation`

## `punctuation`

- `separator`
  - `continuation`
- `terminator`
- `accessor`
- `punctuation.definition.comment`
- `punctuation.definition.keyword`
- `punctuation.definition.annotation`
- `punctuation.definition.string.begin`
- `punctuation.definition.string.end`
- `punctuation.definition.variable`
- `punctuation.section.block.begin`
- `punctuation.section.block.end`
- `punctuation.section.braces.begin`
- `punctuation.section.braces.end`
- `punctuation.section.group.begin`
- `punctuation.section.group.end`
- `punctuation.section.parens.begin`
- `punctuation.section.parens.end`
- `punctuation.section.brackets.begin`
- `punctuation.section.brackets.end`
- `punctuation.section.interpolation.begin`
- `punctuation.section.interpolation.end`
- `punctuation.section.generic.begin`
- `punctuation.section.generic.end`

## `source`

- `source`
  - `*language-suffix*.embedded`

## `storage`

- `type`
  - `function`
  - `class`
  - `struct`
  - `enum`
  - `union`
  - `trait`
  - `interface`
  - `impl`
- `modifier`

## `string`

- `quoted`
  - `single`
  - `double`
  - `triple`
  - `other`
- `unquoted`
- `interpolated`
- `regexp`
- `other`

## `support`

- `function`
- `class`
- `type`
- `constant`
- `variable`
- `module`
- `other`

## `text`

- `html`
- `xml`

## `variable`

- `parameter`
- `language`
- `other`
  - `readwrite`
  - `member`
  - `constant`
- `function`
- `annotation`
