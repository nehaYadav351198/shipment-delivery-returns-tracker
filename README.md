# Shipment Delivery & Returns Tracker (Excel)

A tracker that measures delivery performance against SLA and analyses returns / RTO (Return To Origin), the kind of delivery-timeline and returns reporting an E-commerce MIS team does.

> Data is **simulated** (800 shipments, 4 couriers, 10 cities, 01 Jul - 30 Sep 2026) for practice.

![Summary](screenshots/summary.png)

## What is inside
| Sheet | Contents |
|-------|----------|
| Dashboard | 6 KPI cards and 4 charts (courier on-time %, return reasons, status, city TAT) |
| Summary Tables | Courier scorecard, return / RTO reasons and city-wise delay tables |
| Tracker | Shipment data with dropdowns; SLA, TAT, delay flag and days delayed are automatic |
| Settings | SLA days per city and dropdown lists (editable) |
| About | Definitions and how to use |

## Features
- **Data validation** dropdowns for City, Courier, Status and Reason.
- **SLA lookup** with `VLOOKUP` from the Settings sheet; change an SLA and everything updates.
- **TAT** = Delivery Date - Ship Date; **Delayed** if TAT > SLA.
- **Conditional formatting:** Delayed in red, On Time in green, RTO in red, In Transit in yellow.
- Courier scorecard using `COUNTIFS` and `AVERAGEIFS`.

## Key insights from the data
- Overall on-time delivery is 60.7% and average TAT is 3.7 days.
- **Courier A is the best at 74.5% on-time; Courier C is the weakest at 43.0%.**
- "Refused at delivery" and "Address issue" are the biggest return / RTO reasons (about 25% each), so address verification and order confirmation calls could reduce RTO.
- Remote and Tier-2 cities have higher average TAT than metros.

## Excel skills used
`VLOOKUP`, `IF`, `IFERROR`, `COUNTIFS`, `AVERAGEIFS`, data validation, conditional formatting, charts, freeze panes and filters.
