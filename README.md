# Main Information
- **App Name:**    LasSee
- **Environment:**    MATLAB
- **Author:**    Mostafa Abbasi
- **E-mail:**    [*abbasi.mstfa@gmail.com*](abbasi.mstfa@gmail.com)


# What is LasSee
**LasSee** is a simple and easy-to-use MATLAB app for viewing, subselecting and exporting well-log data from standard LAS files. This app is developed using the `readlas` toolbox [1](https://www.crewes.org/Documents/ResearchReports/2013/CRR201331.pdf) which is a CREWES subproject.

# Main Features
## View LAS-File Contents
Ones the file(s) are added into the app, one may easily see:
- Number of logs included in each file
- Logs statistics (min, max and mean)
- Log plots
- Log values
- LAS header

## Import Logs into MATLAB Workspace
Logs are stored into wells and wells, in turn, are stored into a single database structure called `welldb`. This well database is then imported into the MATLAB workspace. User may edit the well name corresponding to each LAS-file in the Files Table in the app. All the LAS-files that share the same well name, will be stored into single well under the `welldb` structure.

## Export (Save) Logs 
Another option is to export well-logs contents into different file formats on the storage. The supported file formats are as follows:
- **MATLAB data format (*.mat*):** The exported MAT-file includes a single structure variable identical to the one that is imported to the workspace. 
- **Excel Worksheet(*.xls* or *.xlsx*):** All the well-logs assigned into a well are stored into a separate Excel sheets. Thus the exported Excel file will includes as many sheets as the the wells.
- **Comma-Separated Values (*.csv*):**: All the well logs assigned into each well, will be stored into a separate comma-separated ASCII files.
- **Text File (*.txt*):**: All the well logs assigned into each well, will be stored into a separate tab-delimited ASCII TXT-files. 
- **Data File (*.dat*):**: All the well logs assigned into each well, will be stored into a separate tab-delimited ASCII DAT-files. 

## Subselecte Data
Log data may subselected for importing into MATLAB workspace or saving into the storage. Date subselection may be applied in twe forms:
- **subselect by logs names:** User may choose desired well logs by checking the corresponding checkbox next to each log name in the Well-Logs Table.
- **subselect by depth range:** User may define the desired depth range by setting the *Min* and *Max* values in the Files Table.


