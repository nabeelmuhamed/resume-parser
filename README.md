<h1>Resume Parser with Python</h1>
<h4></h4>Introduction</h4>
This document provides an overview of a Python script designed to parse resumes in PDF format. The script extracts information such as name, email, phone number, and skills from multiple PDF files, creates a DataFrame to organize the data, and displays the results.

<h3>Requirements</h3>
--Python (version 3.x)<br>
--PyPDF2 library<br>
--pandas library<br>

You can install the required libraries using the following commands:
**pip install PyPDF2 pandas**<br>
<br>
<h3>Script Overview</h3>
The script consists of the following components:

**extract_text_from_pdf(pdf_path)**: This function takes the path to a PDF file and extracts text from each page.
Information Extraction Function:

**extract_information(text)**: Extracts name, email, and phone number from the extracted text using regular expressions.
Skills Extraction Function:

**extract_skills(text, required_skills)**: Searches for a list of user-defined skills in the extracted text and returns the found skills.
Main Function:

**main()**: Prompts the user to enter the folder path containing PDF files and the skills they are looking for. It processes each PDF, extracts information and skills, and creates a DataFrame.
DataFrame Creation:

The script creates a DataFrame containing columns for PDF name, name, email, phone number, user-defined skills, total skills found, and the total number of user-defined skills.
Displaying the DataFrame:

The final DataFrame is displayed to the user.<br>
<br>
<h3>How to Use</h3>
--Run the script in a Python environment.
--Enter the folder path where your PDF files are located.
--Enter the skills you are looking for (comma-separated).
--View the DataFrame with extracted information and skills.

<h3>Notes</h3>

--Make sure to have the necessary permissions to read the specified folder and files.
--The script uses regular expressions for information extraction, which may need adjustments based on variations in resume formats.
