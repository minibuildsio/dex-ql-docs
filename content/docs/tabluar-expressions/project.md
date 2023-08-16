---
title: "project"
date: 2020-10-06T08:48:57+00:00
lastmod: 2020-10-06T08:48:57+00:00
draft: false
images: []
menu:
  docs:
    parent: "tabluar-expressions"
weight: 100
toc: true
---

Convert an input row to an output row by keeping, dropping, or transforming rows.

## Syntax

```
project Column [= Expression], ...
```
## Parameters

| Name | Type | Required | Description |
| --- | --- | --- | --- |
| Column | column | Yes | The column to appear in the output. |
| Expression | expression | No | An expression to calculate the value |

## Example

The following example will create an output table with columns date identical to the input and distance calculated as 0.00075 * steps.

```
Steps
| project date, distance = steps * 0.00075
```
