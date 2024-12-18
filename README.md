# Web Scraping Project for Company Contact Information

This project focuses on extracting valuable contact information for companies from a large dataset containing 25,000 company names. The primary goal is to automate the process of gathering **email addresses**, **phone numbers**, and **website URLs** for these companies by utilizing **Python** and web scraping techniques.  

## Key Features  
- **Automated Website Discovery**:  
  The script locates the official website for each company using the provided company names and a search engine query mechanism.  

- **Contact Information Extraction**:  
  - **Email Extraction**:  
    Emails are matched to the company domain using a custom "best match" algorithm, ensuring high accuracy.  
  - **Phone Number Detection**:  
    Comprehensive **regular expressions (regex)** are used to extract valid phone numbers from web pages.  

- **Data Storage**:  
  Extracted data is stored in an **SQLite database** for easy access and scalability. For companies where contact information is unavailable, a default value of `"Not Found"` is recorded.  

## Workflow  
1. **Input Dataset**:  
   The project uses an Excel file containing a list of company names as input.  

2. **Web Scraping Pipeline**:  
   - Locate the company website.  
   - Scrape the relevant pages for email addresses and phone numbers.  
   - Validate and clean the extracted data.  

3. **Data Storage and Reporting**:  
   - Save the data in SQLite.  
   - Generate logs for missing or incomplete entries.  

## Tools and Libraries  
- **Python**: The core language for development.  
- **BeautifulSoup**: For parsing HTML content.  
- **Requests**: For making HTTP requests.  
- **Regex**: For pattern matching and data extraction.  
- **SQLite**: For local data storage.  
- **Pandas**: For handling the input dataset and data cleaning.  

## Use Cases  
- Businesses looking to build B2B contact lists.  
- Researchers collecting structured contact information.  
- Automating repetitive data collection tasks for large datasets.  

## How to Use  
1. Clone the repository:  
   ```bash  
   git clone https://github.com/your-repo-name/web-scraping-project.git  
