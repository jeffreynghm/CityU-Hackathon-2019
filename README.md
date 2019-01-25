City University Hackathon 2019 
=============
Task: Extract Information from Annual Report for Account Opening Purpose 
=============

## Information to be extracted
  1. Legal Entity Name
  2. Auditor:
      1. Audit Period
      2. Auditor Opinion
      3. Name of Auditor
  3. Current Year Group Consolidated Financials:
      1. Total Income
      2. Net Profit
      3. Total Equity
   4. Currency of financial items

## Data Description
Data Source: Publicly available annual reports in Singapore Stock Exchange

Training dataset: 40 annual reports (PDF, HOCR, Information tagged JSON)

Testing dataset: 4 annual reports (PDF, HOCR)

### PDF
Downloaded from Singapore Stock Exchange (http://www.sgx.com/)

![picture alt](https://github.com/kelvinyinhei/CityU-Hackathon/blob/master/ReadMe_pictures/Picture_PDF.png)

### HOCR
HOCR is the output from optical character recognition tool, Tesseract OCR. It includes text recognized and coordinates of bounding box of the text.

![picture alt](https://github.com/kelvinyinhei/CityU-Hackathon/blob/master/ReadMe_pictures/Picture_HOCR.png)

### Information tagged JSON
We tag the information manually to identify the type and bounding box for each piece of information in the pages of Independent Auditor Report and Financial Statement

![picture alt](https://github.com/kelvinyinhei/CityU-Hackathon/blob/master/ReadMe_pictures/Picture_JSON.png)

## Deliverables
1. Submit your code to the GitHub repository https://github.com/cityu-hall2/CityHack2019_submissions

2. Presentation
    1. Run the application to extract information from the 4 testing annual reports
        * Not compulsory to have an user interface
    2. Answer the following questions
        * How do you prioritize the information extracted?
        * Explain on the distribution of work between your team
