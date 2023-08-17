---
title: "where"
draft: false
images: []
menu:
  docs:
    parent: "tabular-expressions"
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
