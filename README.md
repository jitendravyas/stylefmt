> Modern CSS Formatter

<div align="center">
  <a href="https://github.com/morishitter/stylefmt">
    <img width=360px src="http://morishitter.github.io/stylefmt-logo.svg">
  </a>
</div>
<br>


## stylelint rules that stylefmt can handle

stylefmt :heart: stylelint

stylefmt supports the following stylelint rules:

- [at-rule-empty-line-before](https://github.com/stylelint/stylelint/tree/master/lib/rules/at-rule-empty-line-before) ("always"|"never" and except "blockless-group" only)
- [at-rule-semicolon-newline-after](https://github.com/stylelint/stylelint/tree/master/lib/rules/at-rule-semicolon-newline-after)
- [block-closing-brace-newline-after](https://github.com/stylelint/stylelint/tree/master/lib/rules/block-closing-brace-newline-after)
- [block-closing-brace-newline-before](https://github.com/stylelint/stylelint/tree/master/lib/rules/block-closing-brace-newline-before)
- [block-opening-brace-newline-after](https://github.com/stylelint/stylelint/tree/master/lib/rules/block-opening-brace-newline-after)
- [block-opening-brace-newline-before](https://github.com/stylelint/stylelint/tree/master/lib/rules/block-opening-brace-newline-before)
- [block-opening-brace-space-after](https://github.com/stylelint/stylelint/tree/master/lib/rules/block-opening-brace-space-after)
- [block-opening-brace-space-before](https://github.com/stylelint/stylelint/tree/master/lib/rules/block-opening-brace-space-before)
- [color-hex-case](https://github.com/stylelint/stylelint/tree/master/lib/rules/color-hex-case)
- [color-hex-length](https://github.com/stylelint/stylelint/tree/master/lib/rules/color-hex-length)
- [declaration-block-properties-order](https://github.com/stylelint/stylelint/tree/master/lib/rules/declaration-block-properties-order)
- [declaration-colon-space-after](https://github.com/stylelint/stylelint/tree/master/lib/rules/declaration-colon-space-after)
- [declaration-colon-space-before](https://github.com/stylelint/stylelint/tree/master/lib/rules/declaration-colon-space-before)
- [declaration-empty-line-before](https://github.com/stylelint/stylelint/tree/master/lib/rules/declaration-empty-line-before)
- [indentation](https://github.com/stylelint/stylelint/tree/master/lib/rules/indentation)
- [length-zero-no-unit](https://github.com/stylelint/stylelint/tree/master/lib/rules/length-zero-no-unit)
- [number-leading-zero](https://github.com/stylelint/stylelint/tree/master/lib/rules/number-leading-zero)
- [number-no-trailing-zeros](https://github.com/stylelint/stylelint/tree/master/lib/rules/number-no-trailing-zeros)
- [selector-combinator-space-after](https://github.com/stylelint/stylelint/tree/master/lib/rules/selector-combinator-space-after)
- [selector-combinator-space-before](https://github.com/stylelint/stylelint/tree/master/lib/rules/selector-combinator-space-before)
- [selector-list-comma-newline-after](https://github.com/stylelint/stylelint/tree/master/lib/rules/selector-list-comma-newline-after)
- [selector-list-comma-newline-before](https://github.com/stylelint/stylelint/tree/master/lib/rules/selector-list-comma-newline-before)
- [selector-list-comma-space-after](https://github.com/stylelint/stylelint/tree/master/lib/rules/selector-list-comma-space-after)
- [selector-list-comma-space-before](https://github.com/stylelint/stylelint/tree/master/lib/rules/selector-list-comma-space-before)
- [shorthand-property-no-redundant-values](https://github.com/stylelint/stylelint/tree/master/lib/rules/shorthand-property-no-redundant-values)
- [string-quotes](https://github.com/stylelint/stylelint/tree/master/lib/rules/string-quotes)

and we can also format from the other stylelint's configration files or packages (e.g. [stylelint-config-standard](https://github.com/stylelint/stylelint-config-standard), [stylelint-config-suitcss](https://github.com/suitcss/stylelint-config-suitcss) and so on) using `extends` property.

## Default formatting rules (without stylelint config file)

### Basic

- 2 spaces indentation - https://stylelint.io/user-guide/rules/indentation/
- require 1 space between a simple selector and combinator
- require 1 space between selectors and `{`
- require new line after `{`
- disallow any spaces between property and `:` https://stylelint.io/user-guide/rules/declaration-colon-space-before/
- require 1 space between `:` and values https://stylelint.io/user-guide/rules/declaration-colon-space-after/
- require new line after declarations
- require `;` in last declaration
- require 1 space between values and `!important`
- disallow any spaces between `!` and `important`
- leave 1 blank line between rules https://stylelint.io/user-guide/rules/rule-empty-line-before/
- leave 1 blank line between rules in atrules https://stylelint.io/user-guide/rules/at-rule-empty-line-before/
- disallow any blank lines between `@import`

### for nested selector syntax

-  leave 1 line between declarations and nested rules

### SCSS

- require 1 space between `@mixin` and mixin name
- require 1 space between mixin name and `(`
- require 1 space between `@extend` and base rules
- require 1 space between `@include` and mixin name
- disallow any spaces between `$variable` and `:`
- require 1 space between `:` and name of variable


## License

The MIT License (MIT)

Copyright (c) 2015 Masaaki Morishita
