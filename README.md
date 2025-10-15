Amazon Samsung Smartwatch Scraper using UiPath

This project automates the process of scraping Samsung Smartwatch data from Amazon.com using UiPath. The extracted data (product names and prices) is then stored in an Excel file for easy analysis.

Overview

The automation performs the following tasks:

Opens Amazon.com in Chrome.

Navigates to the Samsung Smartwatches page.

Extracts product names and prices using UiPath’s Table Extraction feature.

Stores the extracted data in an Excel file.

Tools & Technologies

UiPath Studio (Automation Platform)

Google Chrome (Browser for scraping)

Excel (Data storage)

Steps to Build the Automation

Launch Browser

Use the “Use Application/Browser” activity to open Chrome and navigate to the Amazon Samsung Smartwatches page.

Set Target URL

Provide the Amazon URL of Samsung smartwatches to the browser activity.

Extract Data

Use Table Extraction from UiPath to select and extract multiple product names and their corresponding prices.

Configure selectors properly to ensure all smartwatch listings are captured.

Store Data in Variable

Assign the extracted table to a DataTable variable for further processing.

Write Data to Excel

Use the following Excel activities inside an Excel Process Scope:

Use Excel File → specify the output file path.

Write DataTable to Excel → write the scraped data into the Excel file.

Output

An Excel file (e.g., Samsung_Smartwatches.xlsx) containing the following columns:

Product Name

Price

How to Run

Clone this repository:

git clone repo url


Open the .xaml file in UiPath Studio.

Make sure you have Chrome installed and the UiPath Chrome Extension enabled.

Run the automation. The Excel file with extracted data will be generated in the project folder.

📝 Example Output
Product Name	Price
Samsung Galaxy Watch 6 Classic	12000.00
Samsung Galaxy Watch 5 Pro	17000.00
Samsung Galaxy Watch 4 Bluetooth	21000.00
