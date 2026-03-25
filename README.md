# Basic-N8N-Workflow

Learning the basics of workflow automation with N8N. This project has two workflows that work together, triggering automatically without the need for manual intervention. 

## Workflow 1 - Daily Data Pull: 
Fetches population data for all 50 states from the US Census Bureau API \n
Cleans and transforms the API call into structured fields \n
Adds a column with the run date for historical tracking \n
Checks for data anomalies: flags any state reporting an unusually low population and sends an email alert \n
Appends the data to a Google Sheet

## Workflow 2 - Weekly Summary Report: 
Reads the data set from Google Sheets \n
Isolates the most recent value for each state \n
Sorts states by population (largest to smallest) \n
Formats and sends an email report
