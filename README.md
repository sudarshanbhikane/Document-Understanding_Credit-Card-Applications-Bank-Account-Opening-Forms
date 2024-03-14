
# Document Processing with UiPath Document Understanding: Extracting Fields from Credit Card Applications and Bank Account Opening Forms

A local bank is looking at automating some of their incoming documents to improve the efficiency of the process. The documents lined up for the automation include Credit Card Applications and Bank Account Opening forms.  

The PDF document sent to the respective department includes either the credit card application form or the account opening form. Usually, the account opening form is followed by a Know Your Customer (KYC) form. The order in which these documents are attached in the PDF file may differ. 

We need to extract the fields from the documents and generate a Document Understanding workflow to process the documents by generating the extracted results in Excel files.


## Fields to Extract
### Credit card application

All credit card applications follow a similar structure. It is the only document that you have in the PDF file. You need to extract the following fields from the credit card application
| Field name | Notes     |         Mandatory field
| :-------- | :------- | :----------------------- |
| Card type |	Domestic or international|	Yes   |
| Card variant|	Platinum or Visa |Yes|
|First name| | Yes|
|Middle name| |Yes|
|Last name	|  |Yes|
|Name on card	|  |Yes|
|Mother's maiden name|
|Age	| |Yes
Gender	| Male or Female or Other
Date of birth	
Nationality	| |Yes
Vehicle owned | Car, Two Wheeler
Number of dependants	
Married	
Address	| Address, state, City and Country | Yes |	
Employment status |	Salaried/self-employed/retired | Yes 
Name of the Company	
Designation	
Office address	
Credit cards held | Card No., Issued Bank, and Credit Limit



### Bank account opening process documents

The Account opening form is followed by a Know Your Customer (KYC) form in the same PDF file. The extraction should be done for both document types separately. 

You need to extract the following fields from the account opening form: 

| Field name | Notes     |         Mandatory field
| :-------- | :------- | :----------------------- |
|Customer type |	Public/staff |	Yes
Salutation |	Mr./Mrs./Ms./Other |	
Full name | First, middle, and last name |Yes
Date of birth	| |Yes
Gender |	Male/Female	
Nationality	
Marital status |	Married/Unmarried/Other	
Overseas address	
City	
Country	
Passport details | Passport No, Issue Date, Place of Issue, Nationality, and Date of Expiry|
Applicant signature	| |Yes


#### You need to extract the following fields from the KYC form:
| Field name | Notes     |         Mandatory field
| :-------- | :------- | :----------------------- |
Application type |	New/change request	|
Name of the applicant	| |Yes
Gender	Male/Female	Use checkbox detection	
Marital status |	Single/Married		
Date of birth	
Nationality	| Indian/Other
Residential status |	Resident Individual/ Non- Resident/ Foreign National	
Address for correspondence	
Applicant signature	
