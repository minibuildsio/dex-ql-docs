---
title: "take"
draft: false
images: []
menu:
  docs:
    parent: "tabular-expressions"
weight: 100
toc: true
---

Return up to a specified number of rows.

## Syntax

```
take N
```

## Parameters

| Name | Type | Required | Description |
| --- | --- | --- | --- |
| N | int | Yes | Maximum number of rows to return |

## Example

The following example will return the first 10 rows from the "Steps", if there are fewer than 10 rows in the table all rows will be returned.

```
Steps
| take 10
```
