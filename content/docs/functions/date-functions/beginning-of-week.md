---
title: "beginning_of_week"
draft: false
images: []
menu:
  docs:
    parent: "functions"
weight: 30
toc: true
---

Returns the beginning of the week of the provided date or now if no date is provided.

Monday is the beginning of the week.

## Syntax

```
beginning_of_week([date])
```

## Parameters

| Name | Type | Required | Description |
| --- | --- | --- | --- |
| date | date/datetime | No | A date. Defaults to now if not provided. |

## Example

```
Steps
| project week = beginning_of_week(date)
```