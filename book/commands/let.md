---
title: let
layout: command
version: 0.62.0
usage: |
  Create a variable and give it a value.
---

# `{{ $frontmatter.title }}`

<div style='white-space: pre-wrap;'>{{ $frontmatter.usage }}</div>

## Signature

```> let (var_name) (initial_value)```

## Parameters

 -  `var_name`: variable name
 -  `initial_value`: equals sign followed by value

## Notes
```text
This command is a parser keyword. For details, check
https://www.nushell.sh/book/thinking_in_nushell.html#parsing-and-evaluation-are-different-stages
```
## Examples

Set a variable to a value
```shell
> let x = 10
```

Set a variable to the result of an expression
```shell
> let x = 10 + 100
```

Set a variable based on the condition
```shell
> let x = if false { -1 } else { 1 }
```
