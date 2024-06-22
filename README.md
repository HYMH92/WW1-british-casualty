# WW1 Soldier Details Extraction Tool

This Python project extracts relevant details about deceased soldiers from scanned XML files of British newspapers during World War I. The tool processes these files to identify and extract names, private numbers, and cities of origin, and outputs the data into a structured CSV format.

## Project Overview
The project involves the following steps:

1- Reading XML files: The script reads XML files and extracts text content.
2- Extracting Dates: It identifies and extracts the date of the report.
3- Identifying Relevant Text: The script determines which parts of the text contain relevant information about deceased soldiers.
4- Extracting Soldier Details: From the relevant text, it extracts specific details about each soldier.
5- Saving to CSV: The extracted details are saved into a CSV file for easy analysis.

## Code Breakdown
#### Imports:
- BeautifulSoup: For parsing XML files.
- os: For interacting with the file system.
- numpy: For saving data into CSV format.

#### Constants
- Lists of months and years to help identify dates in the text.

## Functions
  'read_file':
- Reads an XML file, tries multiple encodings, and uses BeautifulSoup to extract text content.

  'get_date':
- Extracts the date (year, month, day) from the list of words.
  
  'get_index':
- Detects relevant text sections that contain information about deceased soldiers.
 
  'relevant_text':
- Extracts relevant text based on the indices identified by get_index.

  'extract_soldier_details':
- Extracts detailed information about each soldier from the relevant text sections.

  'get_directory':
- Generates a list of files in the specified directory.

  'Main Function':
- Put it all togather.
