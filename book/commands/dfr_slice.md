---
title: dfr slice
layout: command
version: 0.62.0
usage: |
  Creates new dataframe from a slice of rows
---

# `{{ $frontmatter.title }}`

<div style='white-space: pre-wrap;'>{{ $frontmatter.usage }}</div>

## Signature

```> dfr slice (offset) (size)```

## Parameters

 -  `offset`: start of slice
 -  `size`: size of slice

## Examples

Create new dataframe from a slice of the rows
```shell
> [[a b]; [1 2] [3 4]] | dfr to-df | dfr slice 0 1
```
