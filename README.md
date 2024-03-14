# Document Processing with UiPath Document Understanding: Extracting Fields from Credit Card Applications and Bank Account Opening Forms

A local bank is looking at automating some of their incoming documents to improve the efficiency of the process. The documents lined up for the automation include Credit Card Applications and Bank Account Opening forms.  

The PDF document sent to the respective department includes either the credit card application form or the account opening form. Usually, the account opening form is followed by a Know Your Customer (KYC) form. The order in which these documents are attached in the PDF file may differ. 

We need to extract the fields from the documents and generate a Document Understanding workflow to process the documents by generating the extracted results in Excel files.
## Dependencies

To execute this project successfully, ensure the following dependencies are met:

1. **UiPath Studio**: UiPath Studio is required to open and modify the provided workflow file.

2. ** Packages ** : 
    1. UiPath.DocumentUnderstanding.ML.Activities
    2. UiPath.IntelligentOCR.Activities
    3. UiPath.UIAutomation.Activities
## Installation

To install and utilize this repository, follow these steps:

1. **Clone the Repository**: Clone this repository to your local machine using the following command:

    ```
    git clone https://github.com/your-username/document-processing.git
    ```

2. **Open in UiPath Studio**: Open UiPath Studio and navigate to the location where you cloned the repository.

3. **Configure Dependencies**: Ensure that UiPath Document Understanding is properly configured within UiPath Studio.

4. **Open Workflow**: Open the provided workflow file (`DocumentProcessing.xaml`) within UiPath Studio.

5. **Adjust Settings**: Adjust any necessary settings or configurations within the workflow to match your environment or requirements.

6. **Run the Workflow**: Run the workflow to process the documents and generate Excel files with extracted fields.

## Fields to Extract

### Credit Card Application

For Credit Card Applications, the following fields need to be extracted:

| Field Name            | Notes                         | Mandatory Field |
|-----------------------|-------------------------------|------------------|
| Card Type             | Domestic or International    | Yes              |
| Card Variant          | Platinum or Visa             | Yes              |
| First Name            |                               | Yes              |
| Middle Name           |                               | Yes              |
| Last Name             |                               | Yes              |
| Name on Card          |                               | Yes              |
| Mother's Maiden Name  |                               |                  |
| Age                   |                               | Yes              |
| Gender                | Male, Female, Other          |                  |
| Date of Birth         |                               |                  |
| Nationality           |                               | Yes              |
| Vehicle Owned         | Car, Two Wheeler             |                  |
| Number of Dependents  |                               |                  |
| Married               |                               |                  |
| Address               | Address, State, City, Country| Yes              |
| Employment Status     | Salaried, Self-employed, Retired | Yes           |
| Company Name          |                               |                  |
| Designation           |                               |                  |
| Office Address        |                               |                  |
| Credit Cards Held     | Card Number, Issuing Bank, Credit Limit |      |

### Bank Account Opening Process Documents

For Bank Account Opening forms, the following fields need to be extracted:

| Field Name             | Notes                               | Mandatory Field |
|------------------------|-------------------------------------|------------------|
| Customer Type          | Public, Staff                       | Yes              |
| Salutation             | Mr., Mrs., Ms., Other               |                  |
| Full Name              | First, Middle, Last Name            | Yes              |
| Date of Birth          |                                     | Yes              |
| Gender                 | Male, Female                        |                  |
| Nationality            |                                     | Yes              |
| Marital Status         | Married, Unmarried, Other           |                  |
| Overseas Address       |                                     |                  |
| City                   |                                     |                  |
| Country                |                                     |                  |
| Passport Details       | Passport Number, Issue Date, Place of Issue, Nationality, Date of Expiry | |
| Applicant Signature    |                                     | Yes              |

### KYC Form

For the KYC Form accompanying the Bank Account Opening form, the following fields need to be extracted:

| Field Name             | Notes                               | Mandatory Field |
|------------------------|-------------------------------------|------------------|
| Application Type       | New, Change Request                 |                  |
| Name of the Applicant  |                                     | Yes              |
| Gender                 | Male, Female                        |                  |
| Marital Status         | Single, Married                    |                  |
| Date of Birth          |                                     |                  |
| Nationality            | Indian, Other                       |                  |
| Residential Status     | Resident Individual, Non-Resident, Foreign National |     |
| Address for Correspondence |                                |                  |
| Applicant Signature    |                                     | Yes              |

## Usage

To utilize this workflow:

1. Ensure that UiPath Studio is installed.
2. Open the provided workflow file.
3. Configure the necessary Document Understanding activities for field extraction.
4. Run the workflow to process the documents and generate Excel files with extracted fields.

## Conclusion

With this UiPath Document Understanding workflow, the bank can streamline its document processing tasks, improving efficiency and accuracy in handling Credit Card Applications and Bank Account Opening forms.
```
