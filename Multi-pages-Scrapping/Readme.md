Multi-Page Web Scraping using UiPath

This project demonstrates how UiPath RPA can be used to perform multi-page web scraping by navigating through multiple product pages and extracting structured data into an Excel file.

The automation scrapes book data from the demo website:
https://books.toscrape.com/

Objective:

- Extract book data from multiple pages automatically  
- Navigate into each product detail page  
- Collect required fields and store them in Excel  
- Convert unstructured web data into structured format  

Target Website:

https://books.toscrape.com/

This website contains multiple book listings with individual product detail pages.

Tools & Technologies:

- UiPath Studio  
- Google Chrome  
- Excel  
- Robotic Process Automation (RPA)

Extracted Data Fields:

The automation extracts the following details:

- Price  
- Book Details Page URL  
- Title  
- UPC  
- Availability  

All extracted data is saved into an Excel file named:
Books_details.xlsx

Workflow Explanation:

1. The bot opens the website using Chrome and navigates to the book listing page.  
2. Table data is extracted from the main page which contains product URLs and prices.  
3. Columns are added to store Title, UPC, and Availability values.  
4. A loop (For Each Row) iterates through each book record.  
5. The bot navigates to the individual product page using the extracted URL.  
6. Required fields (Title, UPC, Availability) are extracted using Get Text activities.  
7. Extracted values are assigned to the corresponding DataTable row.  
8. The complete DataTable is written to an Excel file using Write Range activity.

Output:

The final output is stored as an Excel file with structured data:

- Price  
- Details Page URL  
- Title  
- UPC  
- Availability  

This allows easy analysis and reporting.

How to Run:

1. Open the project in UiPath Studio  
2. Make sure Chrome browser is installed  
3. Update the URL variable if needed  
4. Click Run  
5. Wait for execution to complete  
6. Check the generated Excel file

Use Case:

This project is useful for:

- Learning web scraping with UiPath  
- Understanding multi-page navigation automation  
- Practicing DataTable handling  
- Building real-world RPA automation projects  
