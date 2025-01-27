# PDF Insurance Policy Data Extractor
This Python script is designed to extract specific insurance policy details from a PDF file and save them into an Excel file. It uses the PyPDF2 library to extract text from the PDF and regular expressions (re) to extract relevant details such as the policyholder's name, policy number, premium, and more. Finally, the extracted data is saved into an Excel file using pandas.

# Features
Extracts policyholder name, policy number, policy start and end dates, No Claim Bonus (NCB), Insured Declared Value (IDV), and premium details.
Saves the extracted information into an Excel file for easy access and analysis.
Easy to use with minimal configuration.
# Prerequisites
Before running the script, make sure you have the following Python libraries installed:

PyPDF2: For extracting text from PDF files.
pandas: For saving the extracted data into an Excel file.
```bash
pip install PyPDF2 pandas

```
# Usage
1. Place the policy.pdf file
Ensure the PDF file you wish to extract data from is placed in the same directory as the script or provide the correct file path.

2. Running the script
After setting up the required libraries and placing the PDF file in the correct directory, you can run the script. The script will process the PDF and save the extracted details to an Excel file (policy_details.xlsx) in the same directory.
```bash
python extract_policy_info.py

```
3. Extracted Information
The script will attempt to extract the following details from the policy:

Name: The name of the policyholder.
Policy Number: The unique identifier of the policy.
Policy Start Date: The start date of the insurance policy.
Policy End Date: The end date of the insurance policy.
No Claim Bonus (NCB): The percentage and value of any no-claim bonus.
Insured Declared Value (IDV): The total value of the vehicle.
Premium Net: The net premium for the policy.
GST: The GST amount applied to the premium

4. Output
The extracted data will be saved in an Excel file (policy_details.xlsx) in the current directory. The file will contain the policy details in tabular form.

Example Output
![Screenshot 2025-01-27 234930](https://github.com/user-attachments/assets/cad214da-ef96-458f-bb92-115ce7f92d97)

# Error Handling
If an error occurs during PDF text extraction, it will be printed in the console.
If specific details cannot be found in the PDF, they will not be included in the output file.
# Contributing
Feel free to fork and contribute improvements to the script. Pull requests are welcome for bug fixes, feature requests, or general improvements.
