# Report
**Management :material-menu-right: Report**

View and download **Reports** which provide extensive insights on historical data such as by Customers or Provider routes, DTMF Cost, and Per Number metrics. The ability to Schedule reports adds automation for frequent data requirements.  

!!! tip "Creating additional reports"
    The **Developer :material-menu-right: [Analytics](https://docs.connexcs.com/developers/analytics/)** section of ConnexCS allows providers to manage these reports and create new reports.

## Breakout
The **Breakout** report lists account customers with associated profits, and relevant data such as how much each customer costs, how much they have been charged, ASR and ACD, and so on. The information is here is from processed CDR and so is considered "billing accurate", meaning this data can be used to bill customers. 

+ Use the fields at the top of the page to filter by Customers and Providers, as well as by date range. Each individual column can also be filtered directly in the grid. 
+ Use the Columns and Filters to manage how data is presented. 
+ Enable Pivot Mode (check box at the top of Columns) to setup Row Groups and Values for additional report customization. 

Example: Drag Provider and Provider Destination to Row Groups to see which routes a provider is using for your calls. 

!!! info "Refreshing the Breakout Report"
    Remember to click the refresh button each time parameters change to ensure you see the most recent selections onscreen. When refreshing the list (typically done after modifying the filtering parameters), use the Report Refresh and not the Browser refresh button. 
    
## DTMF
Use the **DTMF** report for customers that send DTMF (ex: voice broadcast systems). This allows you to establish cost effectiveness for a route, and the cost per DTMF digit. 

## Reports
Currently this provides the same functionality and options as the individual Breakout and DTMF reports. Eventually they will be replaced by this page and additional reports will be added. This page has the same Pivot and Filtering functionality as the **Breakout** report. 

## Per Number
This report displays metrics for a specific number. It is particularly useful if you get a complaint about people dialing a specific number. Select the number and define the time frame (max 6 months) to generate a list of all calls for that number, along with call details. Click **`Numbers`** to search for multiple numbers. 

## Schedule Report
This feature emails the Breakout Report at designated intervals. To schedule a breakout report: 

1. Click the **`+`** icon.

    ![alt text][schedulereport]

2. **Name** the report schedule.
3. **Email**: The report recipient. 
4. **Group**: Select one or more ways to group the data.
5. **Customers**: Select one or more, or leave it blank for all Customers. 
6. **Providers**: Select one or more, or leave it blank for all Providers. 
7. **Columns**: Select the columns to include in the report. 
4. Click **`Save`**.

[schedulereport]: /reports/img/schedulereport1.png "Schedule Reports"
