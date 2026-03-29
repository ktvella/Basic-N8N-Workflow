# Basic n8n Workflow

Learning the basics of workflow automation with N8N. This project has two workflows that work together, triggering automatically without the need for manual intervention. 

## Workflow 1 - Daily Data Pull 
Fetches population data for all 50 states from the US Census Bureau API <br>
Cleans and transforms the API call into structured fields <br>
Adds a column with the run date for historical tracking <br>
Checks for data anomalies: flags any state reporting an unusually low population and sends an email alert <br>
Appends the data to a Google Sheet

## Workflow 2 - Weekly Summary Report
Reads the data set from Google Sheets <br>
Isolates the most recent value for each state <br>
Sorts states by population (largest to smallest) <br>
Formats and sends an email report
