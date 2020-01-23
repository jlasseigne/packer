---
layout: "docs"
page_title: "list - Functions - Configuration Language"
sidebar_current: "configuration-functions-collection-list"
description: |-
  The list function constructs a list from some given elements.
---

# `list` Function


~> **This function is deprecated.** From Packer v0.12, the Packer
language has built-in syntax for creating lists using the `[` and `]`
delimiters. Use the built-in syntax instead. The `list` function will be
removed in a future version of Packer.

`list` takes an arbitrary number of arguments and returns a list containing
those values in the same order.

## Examples

```
> list("a", "b", "c")
[
  "a",
  "b",
  "c",
]
```

Do not use the above form in Packer v0.12 or above. Instead, use the
built-in list construction syntax, which achieves the same result:

```
> ["a", "b", "c"]
[
  "a",
  "b",
  "c",
]
```
