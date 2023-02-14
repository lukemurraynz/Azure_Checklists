
# Azure Architecture - Solution requirement considerations

Blog post can be found here: [Azure Architecture - Solution Requirement Consideration Checklist](https://luke.geek.nz/azure/azure-architecture-solution-requirement-consideration-checklist/)

Quick links for using the checklists in this repo:

- [Latest release of the Excel spreadsheet](https://github.com/Azure/review-checklists/releases/latest/download/review_checklist.xlsm)

Summary of checklists supported and the respective responsible owners:

- [azure_architecture_checklist.en](https://github.com/lukemurraynz/Azure_Checklists/blob/main/azure_architecture_checklist.en.json)

## What is an Azure Architecture - Solution requirement considerations?

Building a cloud solution on Azure can be an exciting yet daunting task.

The key to a successful implementation is carefully planning and considering solution requirements using the guidance of the Microsoft Cloud Adoption and Well Architecture frameworks.

But knowing what questions to ask and data to capture to give you the bigger picture - to not only consider the solution for the short term and long term, can be difficult.

Leaning on the great frameworks already in place to assist with the [Cloud Adoption](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/?WT.mc_id=AZ-MVP-5004796) and [Azure Well Architecture frameworks](https://learn.microsoft.com/en-us/azure/architecture/framework/?WT.mc_id=AZ-MVP-5004796), the solution requirements checklist is intended to act as a way of asking and capturing the requirements of your solutions. It can be a great reminder to discover some of those requirements (whether functional or non-functional) that you may have forgotten about!

## Why this repository?

This repo separates the actual checklist contentfrom the offical/community driven checklists offered as part of the [Azure Review Checklist](https://github.com/Azure/review-checklists). This checklist is aimed as a method of capturing business requirements before the review stage.

## Reporting errors and contributing

Please feel free to open an issue or create a PR if you find any error or missing information in the checklist. This is aimed to be community driven.

## Using the spreadsheet for Azure reviews

1. Download the Excel spreadsheet from the [latest release](https://github.com/Azure/review-checklists/releases/latest/download/review_checklist.xlsm) to your PC

2. Download the latest version of the Azure architecture JSON file to your computer.

3. In the Fastrack for Azure Review Checklist, select Import Checklist from JSON.

4. Import the checklist.

5. (Optional) If you are going to distribute the spreadsheet to users that cannot work with macros (for example, either because of security reasons or because they use Office for Mac), save a version of the spreadsheet in xlsx format (instead of xlsm). Note that disabling macros will result in the spreadsheet losing its ability to import updated versions of the checklist or JSON-based Azure Resource Graph query results

6. Go row by row, and set the "Status" field to one of the available options, and write any remarks in the "Comments" field (such as why a recommendation is not relevant, or who will fix the open item)

   1. Since there are many rows in a review, it is recommended proceeding in chunks: either going area after area (first "Networking", then "Security", etc) or starting with the "High" priority elements and afterwards moving down to "Medium" and "Low"
   1. If any recommendation is not clear, there is a "More Info" link with more context information.
   1. **IMPORTANT**: design decisions are not a checkbox exercise, but a series of compromises. It is OK deviating from certain recommendations, if the implications are clear (for example, sacrificing security with operational simplicity or lower cost for non-critical applications)

7. Check the "Dashboard" worksheet for a graphical representation of the review progress

## Security settings running macros

There are some settings that you might need to change in your system to run macro-enabled Excel spreadsheets. When initially opening the file you may see the following error, which prevents Excel from loading:

> Excel cannot open the file 'review_checklist.xlsm' because the file format or file extension is not valid. Verify that the file has not been corrupted and that the file extension matches the format of the file.

In other cases the file opens with the following message, which prevents you from being able to load the checklist items:

### Unblock file or add an exception to Windows Security

1. You might need to unblock the file from the file properties in the Windows File Explorer, so that you can use the macros required to import the checklist content from github.com:

2. Additionally, you might want to add the folder where you cloned this repo to the list of exceptions in Windows Security (in the Virus & Threat Protection section):

## Disclaimer

- This is not official Microsoft documentation or software.
- This is not an endorsement or a sign-off of an architecture or a design.
- This code-sample is provided "AS IT IS" without warranty of any kind, either expressed or implied, including but not limited to the implied warranties of merchantability and/or fitness for a particular purpose.
