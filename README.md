# Generate Yearly Report
RPA project designed as one of the tests of the UiPath Advanced Course.

Process that:

- Open the ACME System 1 web application (https://acme-test.uipath.com). 
- Access the Dashboard - the central location, where the user can pick a specific menu item.
- Log in to System 1. Required input data: email and password.
- Access the Work Items Listing to view all the available tasks to be performed (Output data: list of tasks).
- For each activity of the WI4 type perform the following steps:
  - Open the Details page of the selected activity to retrieve the Vendor Tax ID (Output data: TaxID). 
  - Go back to the Dashboard and access the Download Monthly Report section in the Reports menu.
  - Fill in the Vendor TaxID and download all the corresponding monthly reports from the last year.
  - Group all the downloaded monthly reports into a single Excel yearly report with the “Yearly-Report-2017-TAXID.xlsx” name.
  - Fill in the Vendor TaxID, set the year as 2017, and select the file on your hard drive. This will return a unique upload ID. Out upload ID.
  - Upload the resulting Excel yearly report in the “Upload Yearly Report” section in the Reports menu.
  - Go back to the Work Item Details page and select Update Work Item.
- Continue with the next WI4 activity.

Obs.: This process uses the REFramework inside the UiPath.

For more information regarding the process needs, see the document "Generate Yearly Report - Process Design Document.pdf"
