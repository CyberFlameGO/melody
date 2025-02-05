---
sidebar_position: 6
---

# Syntax

## Keywords

- `of` - used after a number or a range and before a sequence to be matched, e.g. `5 of "A";`, equivalent to regex `{5}`
- `to` - used to create a range (either as a quantifier or as a character range), e.g. `5 to 9`, equivalent to regex `{5,9}` if before an `of` or `[5-9]` otherwise
- `capture` - used to open a `capture` or named `capture` block, equivalent to regex `(...)`
- `match` - used to open a `match` block, equivalent to regex `(?:...)`
- `either` - used to open an `either` block, equivalent to regex `(...|...)`
- `some` - used with `of` to express 1 or more of a pattern, equivalent to regex `+`
- `over` - used with `of` to express more than an amount of a pattern, equivalent to regex `{6,}` (assuming `over 5 of ...`)
- `option` - used with `of` to express 0 or 1 of a pattern, equivalent to regex `?`
- `any` - used with `of` to express 0 or more of a pattern, equivalent to regex `*`

## Symbols

- `<start>` - matches the start of the string, equivalent to regex `^`
- `<end>` - matches the end of the string, equivalent to regex `$`
- `<char>` - matches a single character, equivalent to regex `.`
- `<space>` - equivalent to regex `\s`
- `not <space>` - equivalent to regex `\S`
- `<newline>` - equivalent to regex `\n`
- `<tab>` - equivalent to regex `\t`
- `<return>` - equivalent to regex `\r`
- `<feed>` - equivalent to regex `\f`
- `<null>` - equivalent to regex `\0`
- `<digit>` - equivalent to regex `\d`
- `not <digit>` - equivalent to regex `\D`
- `<vertical>` - equivalent to regex `\v`
- `<word>` - equivalent to regex `\w`
- `not <word>` - equivalent to regex `\W`

## Literals

- `"..."` or `'...'` - used to mark a literal part of the match. Melody will automatically escape characters as needed. Quotes (of the same kind surrounding the literal) should be escaped

## Raw

- <code>\`...\`;</code> - added directly to the output without any escaping

## Comments

- `//` - used to mark comments
