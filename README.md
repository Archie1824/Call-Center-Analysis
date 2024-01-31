# Call Center Trends

## Problem Statement

The project aims to design and implement a dynamic Power BI report for telecome company, enabling them to efficiently monitor and analyze key performance indicators (KPIs) and metrics related to customer service operations. The report will provide actionable insights to optimize operational efficiency, enhance customer satisfaction, and improve agent performance.

### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : Perform data cleaning tasks such as removing duplicates, filtering out irrelevant rows or columns, and correcting data inconsistencies.
- Step 5 : Create measures using DAX formulas to derive new metrics and KPIs from the raw data. Here is a list of measures created using DAX:
 
    Total calls answered = CALCULATE(COUNTROWS('Call center'), 'Call center'[Total number of calls] = "Y")

    Total calls abandoned = CALCULATE(COUNTROWS('Call center'), 'Call center'[Total number of calls] = "N")

    Average speed of answer in seconds = Average('Call center'[Speed of answer in seconds])

    Average satistafction rate = Average('Call center'[Satisfaction rating])

    Average call duration = Average('Call center'[AvgTalkDuration])

- Step 6 : In the report view, under the view tab, theme was selected.
- Step 7 : Drag and drop visualizations from the Visualizations pane onto the canvas to create the initial layout of the dashboard. 
- Step 8 : Arrange the visualizations and organize them into logical groups or sections to facilitate user understanding and navigation.
- Step 9 : Customize the appearance of visualizations by adjusting formatting options, colors, labels, and titles.
