Binlkit Dashboard


1. load the data 
2. Transform Data
3. Total Count Of Rows -- 8523
4. we have to convert----> LF into LOW FAT and REG into REGULAR by replacing values
                           low fat  TO  Low Fat 
                           reg  TO  Regular
5. Data Cleaning is over
6. insert--> shape--> rounded tab, both top --> rotate it to 90 degrees --> enlarge it --> colour change to #FFD200 --> border off --> shadow on 
7. insert --> text box --> add text "blinkit" --> select only "it" and add colour #007EOD --> 
8. insert --> text box --> add text " India's Lat Minute App " and place it below blinkit

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
                                                ****   CREATING KPI CARDS  ****

9. Modeling/ table tools --> new measure --> Total Sales = SUM('BlinkIT Grocery Data'[Sales]) --> click enter
10. modeling --> new measure --> Avg Sales = AVERAGE('BlinkIT Grocery Data'[Sales]) -> click enter
11. modeling --> new measure --> Total Items = COUNTROWS('BlinkIT Grocery Data') --> click enter
12. modeling --> new measure --> Avg rating = AVERAGE('BlinkIT Grocery Data'[Rating]) --> click enter
13. select card --> select total sales, avg rating, total items, avg sales --> format visuals --> layout (grids) --> style (tiles) --> rows (2) --> columns (2)
                   increase the size of the values and the labels : callout --> values --> Segoe UI Bold, 25
                                                                    Label --> position --> Boottom 
                   shadow --> ON , Glow --> ON
14. Add Image to the cards : Cards--> apply settings to --> Total sales --> background --> add image --> adjust transparency and glow 
15. cards -->accent bar --> set colour 
16. callout --> label --> segeo UI semibold
17. add images (icons) to the cards
------------------------------------------------------------------------------------------------------------------------------------------------------------------------
                                                ****  CREATING CHARTS  ****

20. insert --> shape --> rectangle --> style (rounded rectangle) --> background(white) --> border(grey) --> shadow (ON)
21. Modeling --> new parameter --> fields --> add total sales, avg sales, total items, avg rating --> new parameter(slicer) is formed in the table 
                                              arrange it in the rectangle shape --> off slicer header
                                              values --> segoe ui semibold,10, bold
                                              border --> black colour
                                              background --> yellow

22. select donut chart --> SET item fat content in legend & parameter in values
                       --> Do all the format visuals accordingly 

23. select clustered bar chart --> SET outlet location type in y-axis, parameter in x-axis, item fat content in legend
                               --> Do all the format visuals accordingly 

24. select stacked bar chart --> SET item type in y-axis & parameter in x-axis
                             --> Do all the format visuals accordingly

25. copy paste the rectangle shape and make it as the border lines between the charts 

26. add another rectangle shape beside the charts

27. select donut chart --> SET outlet size in legend & total sales in values
                       --> Do all the format visuals accordingly

28. select funnel chart --> SET outlet location type in category & sum of sales in values 
                        --> Do all the format visuals accordingly

29. select line chart --> SET outlet establishment in x-axis & total sales in y-axis
                      --> Do all the format visuals accordingly

30. select matrix chart --> SET outlet type in rows & total sales, avg sales, total items, avg rating, items in values
                        --> Do all the format visuals accordingly

31. select slicer chart --> SET outlet location type in field 
                        --> Do all the format visuals accordingly

32. select slicer chart --> SET outlet size in field
                        --> Do all the format visuals accordingly

33.  select slicer chart --> SET item types in field
                        --> Do all the format visuals accordingly

34. Add "FILTER PANEL" text 

35. insert --> buttons --> blank --> Action (ON) --> page navigation 
                       --> style --> fill --> add image  

36. insert --> buttons --> Reset --> Action (ON) --> back           
                       --> Action (ON) --> bookmark --> Bookmark (reset)

   [ 1.To use reset button u have to first set bookmark : Format --> edit interactions (OFF)- if u select any particular data
      2.View --> bookmark --> ADD --> rename Bookamark with RESET --> update]
                                      
                                 --> --> Action (ON) --> bookmark --> Bookmark (reset)


37. insert --> buttons --> blank --> Action (ON) --> page navigation 
                       --> style --> fill --> add image ( table ) 
  
38. insert --> buttons --> blank --> Action (ON) --> page navigation 
                       --> style --> fill --> add image ( info )
                       --> Action --> tooltip : "Welcome to blinkit"

39. insert --> add text --> " Developed by AnalyticalCK"

40. Add image --> youtube logo

                      










































