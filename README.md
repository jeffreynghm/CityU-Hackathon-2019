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



### HOCR
HOCR is the output from optical character recognition tool, Tesseract OCR. It includes text recognized and coordinates of bounding box of the text. The bounding box of HOCR "bbox" is x0 (left), y0 (top), x1 (right) and y1 (bottom). The classes include "ocr_par", "ocr_line" and "ocrx_word" which are paragraph, line and word. The "x_wconf" is the confidence of recognizing the word.

[HOCR Description](https://en.wikipedia.org/wiki/HOCR)


### Information tagged JSON
We tag the information manually to identify the type and bounding box for each piece of information in the pages of Independent Auditor Report and Financial Statement. The "pt0" and "pt1" are bounding box coordinate of top-left and bottom-right points. The "entityType" is the type of information.



This is how we tagged it.



## Deliverables
1. Submit your code to the GitHub repository 

2. Presentation
    1. Run the application to extract information from the 4 testing annual reports
        * Not compulsory to have an user interface
    2. Answer the following questions
        * How do you prioritize the information extracted?
        * Explain on the distribution of work between your team

# Our Support
You can look for us in the venue or ask questions in



# Agreement and Disclaimer
'Data' means the Data or Datasets linked from the Github repository, “CityU-Hackathon-2019”, for the purpose of use by Participants in the Competition, “CityHack 2019”. For the avoidance of doubt, Data is deemed for the purpose of developing any prototype or executable code by Participants. Participants must use the Data only as permitted by any associated data use rules specified as follows. 

Participants must use the Data solely for the purpose and duration of the Competition, including but not limited to reading and learning from the Data, analyzing the Data, modifying the Data and generally creating your Submission and any underlying models. Participants must not copy, access, store, archive, or otherwise use the Data for any purpose other than to participate in the Competition for which such Data was provided. Participants may not use the data in such a way as to repackage, resell, allow bulk data download, or otherwise similarly exploit the data. Participants agree to use suitable measures to prevent persons who have not formally agreed to the data use rules from gaining access to the Data and agree not to transmit, duplicate, publish, redistribute or otherwise provide or make available the Data to any party not participating in the Competition. Participants agree to notify the owner of the Github repository immediately upon learning of any possible unauthorized transmission or unauthorized access of the Data and agree to work with the owner of the Github repository to rectify any unauthorized transmission. Participants agree that participation in the Competition shall not be construed as having or being granted a license (expressly, by implication, estoppel, or otherwise) under, or any right of ownership in, any of the Data.
