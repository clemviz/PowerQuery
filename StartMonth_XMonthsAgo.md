# StartDate

- Copy/Paste as a Blank Query 
- Return a Date

```M
let
    Today = DateTime.Date(DateTime.LocalNow()),
    Interval_Months = 16,
    FirstDayXMonthsAgo = Date.StartOfMonth(Date.AddMonths(Today, -Interval_Months))
in
    FirstDayXMonthsAgo
```
