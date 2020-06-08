# Expense tracker Excel template
An Excel template for expense manager with sub categories, multiple accounts and reports.

The workbook contains the following sheets,

 1. [Transactions](#Transactions)
 2. [Report (Data)](#Reports)
 3. [Report (Chart)](#Reports)
 4. [Categories](#Masters)
 5. [Sub Categories](#Masters)
 6. [Accounts](#Masters)

Let's dive into each sheet into detail,

### Transactions

This is the sheet where you enter the day to day transactions.

**Date**
 - The values are of Short Date type.

**Transaction Type**
 - There are three transaction types - Expense, Income and Transfer.
 - Data validation is used for the drop-down.
 - The list for data validation is from the top row of the 'Categories' sheet.

**Account**
 - Data validation list is taken from the 'Accounts' sheet.

**Category**
 - Category dropdown appears based on the Transaction Type.
 - Data Validation list is the INDIRECT of the Transaction Type.
 - This works as we have created defined names using the Create from Selection option in 'Categories' sheet before.

**Sub-Category**
 - Sub Categories appear based on the Category selected.
 - This is done just like categories using INDIRECT and defined names.

**Transferred to**
 - Account Name for which the funds are being transferred.

**Amount**
 - Formated as currency.

**Memo**
 - The title is self-explanatory.

### Reports

The reports are divided in two sheets, one for data and another for charts. This sheet contains charts.

 - The fields that are user input are highlighted in Yellow color.
 - There are two report lists here.
 - The first one contains list of expenses and income divided by categories. You can set start date and end date for it.
 - In the second list you can select a category and see the spend across sub categories.

The second workbook contains charts for the same data presented in the first one. So the date change in the first sheet affect the second one too.

### Masters

The masters are put in separate sheets cause it looks nice and is convinent. The masters include the following

 - Transaction Type - As a header in categories sheet.
 - Categories - In categories sheet and a header in Sub categories sheet.
 - Sub categoris - In the sub categories sheet
 - Accounts - In the accounts sheet.