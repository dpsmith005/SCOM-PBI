# SCOM Power BI Templates

SCOMHealth_BLANK.pbit - SCOM health check for administrators.  This is based on a lot of the SQL queries on Kevin Holman's blog.  I use this to check performance metric collections to tune the performance rules.

SCOM_MS_PERF.pbit - Collects performance data for the managment servers and gateways for the past 7 days.  This can be adjusted by changing the SQL query for the hourly and raw data.  Keep in mind that there are limits on these data sets.  The raw performance data we collect is set to 10 days. The hourly data will collect and store data for a longer period of time.

SCOM_Perf_Sample5_NoSG.pbit - A generic performance report for SCOM agents.  This report limits the data to a list of servers based on a group.  Do not select All Windows Computers.  It will try to load a lot of data.  My environment will cause PBI to fail loading the data.
