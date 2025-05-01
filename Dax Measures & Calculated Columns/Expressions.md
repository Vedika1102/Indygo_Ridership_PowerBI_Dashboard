
## Dax Measures:

1. **TotalRidership**
   
       TotalRidership = SUM(FactSegmentAdherence[DepartBoards])

2. **Total Ridership of Previous Week**

       TotalRidership_PreviousWeek =
       VAR SelectedStartDate = MIN('DimDate'[CalendarDate])
       VAR StartOfPreviousWeek = SelectedStartDate - WEEKDAY(SelectedStartDate, 1) - 6
       VAR EndOfPreviousWeek = SelectedStartDate - WEEKDAY(SelectedStartDate, 1)
     
       RETURN
       CALCULATE( [TotalRidership], 
       FILTER(ALL('DimDate'),  
         'DimDate'[CalendarDate] >= StartOfPreviousWeek &&
         'DimDate'[CalendarDate] <= EndOfPreviousWeek ) )

 ## Calculated Columns:

 1. **Route Display Name**
 
        RouteDisplayName = FORMAT('DimRoute'[RouteFareboxID], "0") & " - " & 'DimRoute'[RouteInternetName]

2. **Week Number**

       WeekNum = WEEKNUM('DimDate'[CalendarDate], 2) 


