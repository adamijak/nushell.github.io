---
title: dfr set-with-idx
layout: command
version: 0.62.0
usage: |
  Sets value in the given index
---

# `{{ $frontmatter.title }}`

<div style='white-space: pre-wrap;'>{{ $frontmatter.usage }}</div>

## Signature

```> dfr set-with-idx (value) --indices```

## Parameters

 -  `value`: value to be inserted in series
 -  `--indices {any}`: list of indices indicating where to set the value

## Examples

Set value in selected rows from series
```shell
> let series = ([4 1 5 2 4 3] | dfr to-df);
    let indices = ([0 2] | dfr to-df);
    $series | dfr set-with-idx 6 -i $indices
```
