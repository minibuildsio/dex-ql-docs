---
title: "format_date"
draft: false
images: []
menu:
  docs:
    parent: "functions"
weight: 100
toc: true
---

Returns a string representation of a datetime using a provided format.

## Syntax

```
format_date(date, format)
```

## Parameters

| Name | Type | Required | Description |
| --- | --- | --- | --- |
| date | date/datetime | Yes | A date. |
| format | string | Yes | A format e.g. "yyyy-MM", see table below. |

## Supported Format Symbols

|Symbol|Meaning|Presentation|Examples|
|---|---|---|---|
|G|era|number/text|1; 01; AD; Anno Domini|
|u|year|year|2004; 04|
|y|year-of-era|year|2004; 04|
|D|day-of-year|number|189|
|M|month-of-year|number/text|7; 07; Jul; July; J|
|d|day-of-month|number|10|
|Q|quarter-of-year|number/text|3; 03; Q3|
|Y|week-based-year|year|1996; 96|
|w|week-of-year|number|27|
|W|week-of-month|number|27|
|e|localized day-of-week|number|2; Tue; Tuesday; T|
|E|day-of-week|number/text|2; Tue; Tuesday; T|
|F|week-of-month|number|3|
|a|am-pm-of-day|text|PM|
|h|clock-hour-of-am-pm (1-12)|number|12|
|K|hour-of-am-pm (0-11)|number|0|
|k|clock-hour-of-am-pm (1-24)|number|0|
|H|hour-of-day (0-23)|number|0|
|m|minute-of-hour|number|30|
|s|second-of-minute|number|55|
|S|fraction-of-second|fraction|978|
|A|milli-of-day|number|1234|
|'|escape for text|delimiter|
|''|single quote|literal|'|
## Example

```
Steps
| project year_month = format_date(date, "yyyy-MM")
```