---
title: split row
layout: command
version: 0.62.0
usage: |
  Split a string into multiple rows using a separator
---

# `{{ $frontmatter.title }}`

<div style='white-space: pre-wrap;'>{{ $frontmatter.usage }}</div>

## Signature

```> split row (separator)```

## Parameters

 -  `separator`: the character that denotes what separates rows

## Examples

Split a string into rows of char
```shell
> echo 'abc' | split row ''
```

Split a string into rows by the specified separator
```shell
> echo 'a--b--c' | split row '--'
```
