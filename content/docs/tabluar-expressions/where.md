---
title: "where"
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

Select all rows where the provided condition is true.

## Syntax

```
where Condition
```

## Parameters

| Name | Type | Required | Description |
| --- | --- | --- | --- |
| Condition | expression | Yes | Expression that evaluates to true or false. |

## Example

The following example will return rows where the steps count is 15,000 or more from the current month. 

```
Steps
| where steps >= 15000 and date >= beginning_of_the_month()
```
