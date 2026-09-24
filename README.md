# AtliQ Grands Hospitality Revenue and Occupancy Analysis

An independent Power BI case study using sample hotel data for May–July 2022. The analysis covers 25 properties, 134,590 booking records, and daily capacity and successful-booking data.

## Project goal

Build an interactive report to explore hotel revenue, occupancy, guest ratings, booking channels, and cancellations across properties and cities.

## Tools

- Microsoft Power BI Desktop
- Power Query
- DAX

## Data model and approach

The model keeps individual booking records separate from daily aggregated capacity and successful-booking records. Shared hotel, room, and date dimensions filter both fact tables. This supports booking-level revenue and cancellation analysis alongside occupancy calculations without duplicating capacity.

The report includes filters for city, property, check-in month and week, booking status, and booking platform. Status and platform filters affect booking-based measures; the supplied capacity data has no status or platform breakdown, so those filters do not change occupancy.

## Measures

- Realized revenue
- Total bookings
- Average rating (rated bookings only)
- Total capacity
- Successful bookings
- Occupancy rate
- Cancelled bookings
- Cancellation rate
- Month-over-month changes for revenue, occupancy, and average rating
- Cancellation refund amount
- Realized revenue per booking

## Findings

- Revenue fell 4.8% in June versus May, then rose 3.4% in July versus June. Occupancy declined from 58.5% in May to 57.5% in July.
- Cancellation rates varied little by platform, ranging from about 24.3% to 25.0%. The “others” platform accounted for 40.7% of the calculated cancellation-refund amount, broadly in line with its share of bookings.
- Realized revenue per booking averaged about 15,387 in Mumbai and 9,322 in Hyderabad. This is a descriptive comparison; room mix and stay length may contribute to the difference.

## Notes and limitations

- The reporting period is May–July 2022, based on check-in date.
- The source does not specify a currency, so revenue values are reported in source units.
- May’s month-over-month comparison is unavailable because April check-in data is not included.
- Average rating excludes bookings without a rating.
- The data shows comparisons, not the causes behind them.
