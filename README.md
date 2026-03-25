# Basic-N8N-Workflow

Learning the basics of workflow automation with N8N. This project has two workflows that work together, triggering automatically without the need for manual intervention. 

## Workflow 1 - Daily Data Pull: 
Fetches population data for all 50 states from the US Census Bureau API
Cleans and transforms the API call into structured fields
Adds a column with the run date for historical tracking
Checks for data anomalies: flags any state reporting an unusually low population and sends an email alert
Appends the data to a Google Sheet

## Workflow 2 - Weekly Summary Report: 
Reads the data set from Google Sheets
Isolates the most recent value for each state
Sorts states by population (largest to smallest)
Formats and sends an email report
