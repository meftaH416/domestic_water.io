This file loads data from Standard Building America DHW Schedules (BuildingAmerica_DHW.xlsm) excel files saves in local directory.
Link: https://www.energy.gov/eere/buildings/building-america-analysis-spreadsheets

There are two .ipynb files. The one names waterdata.ipynb creates a new csv file (water.csv) only having hot water data along with times.
Further processes the file and aggregated into 8759 hourly data files of hot water consumption along with graphics.
The Hot Water schedules is necessary for any Solar Hot Water modeling or Building Energy Modeling.

The other python file (excel_python.ipynb) file is an excelent way to use openpyxl library. It loads the BuildingAmerica_DHW.xlsm files with all macros enabled. Then it checks for user inputs using openpyxl dataValidation (dropdown input). User can search for the name of the weather station for which city they are looking for. They can then manually input that city name to python notebook and get the Water Consumption data. The codes saves a new excel file (.xlsm) with all the macros enabled. This new file then can be used to map hourly 8,760 data with datetime and visualize Water useage demand at different hours of a day. 
