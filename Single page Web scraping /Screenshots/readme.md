This project automates the process of extracting structured data about Indian States, including State Name, Capital, Chief Minister, and Governor, from a public website using UiPath. 
The extracted data is automatically saved into an Excel workbook for further analysis or reference.
The automation eliminates manual copy-paste work and ensures accurate, repeatable data extraction using web scraping techniques.
This project is designed to scrape data from a **https://gkchronicle.com/general-knowledge/states-and-their-capitals.php ** website and store the extracted information into an Excel file using UiPath.

The automation process starts by using the Use Application/ Browser activity in UiPath to launch Google Chrome and navigate to the required website URL that contains the data table. Once the webpage is loaded, the Extract Table Data activity is used to identify and scrape the table present on the site. UiPath automatically captures the rows and columns of the table, including details such as state name, capital, chief minister, and governor, and stores this information in a DataTable variable.

After successfully extracting the data, the workflow creates an Excel file using the Write Range (Workbook) activity. The DataTable containing the scraped web data is written into an Excel file named IndianStates.xlsx, starting from the first cell of the selected worksheet. Finally, the browser is closed after the data is saved, completing the automation process. The result is a well-structured Excel file containing accurate data scraped directly from the website.
