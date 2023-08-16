---
title: "sort"
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

Sort the rows in a table by a given column optionally specifying a direction.

## Syntax

```
sort Column [Order]
```

## Parameters

| Name | Type | Required | Description |
| --- | --- | --- | --- |
| Column | column | Yes | The column to sort the table by. |
| Order | asc or desc | No | The order to sort by, defaults to asc i.e. low to high. |

## Example

The following example will sort the table by the steps column in .

```
Steps
| sort steps desc
```
