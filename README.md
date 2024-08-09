**Description**

- The automation project aims to streamline the daily update and distribution of a report summarizing ageing unpaid invoices. Every day, between 12 a.m. and 6 a.m., IT saves a data dump in CSV format to a specific folder. This data is linked to an Excel template file containing a pivot table that organizes the data by customer.
- At 6 a.m., a .bat file will be triggered by the Windows Task Scheduler to open the macro workbook. Upon opening, a VBA macro will execute, refreshing the data connections and pivot table in the template with the latest data. The updated report will then be saved with the current date in the filename. The macro will extract a list of email addresses from a separate file and send the report to the designated recipients.
- The process includes error handling; if any issues arise during execution, an email notification will be sent to the relevant parties. This automated system ensures that the report is consistently updated and distributed without manual intervention, improving efficiency and reliability.