# Settings for the organization

If you are in the context of the organization, you will find the item "Settings" in the main menu on the far right.
Here you can make the settings for the organization. In the settings you have the following subsections:

## Name 

Every organization on ZEIT.IO has a unique name on ZEIT.IO. You can change this unique name here.
You can only choose names that are not already used by another organization on ZEIT.IO.
Changing the name of the organization affects old links.
It is possible that after a name change, old links (URLs) to reports within this organization will no longer work.

## General

Here you can set the following default values for your organization:

- **Currency**: The currency in which the invoices should be created.
- **Tax rate**: The default tax rate to be used for the invoices.
- **Language**: The language in which the ZEIT.IO user interface should be displayed.
- **Holiday prefix for calendar entries**: The prefix to be used for holiday calendar entries.
- **Mandatory field order number**: Here you can configure whether the order number should be a mandatory field for projects.
- **Mandatory field project number**: Here you can configure whether the project number should be a mandatory field for projects.

## Billing address

Here you can store the following data:

- **Industry**: The industry in which your organization operates.
- **Billing address**: The official billing address of your organization. Including legal form, tax number and commercial register number.
- **Contact details**: The general contact details of your organization.
- **Invoice recipient**: An email address for incoming invoices. You will also receive invoices from ZEIT.IO at this email address.

The information here is also used for the footer on outgoing invoices and credit notes created by ZEIT.IO.

## Invoice number

Here you can specify the format for the invoice number that should be used for outgoing invoices.
Credit notes have their own number range that can be configured separately.

### CONSEQUENTIAL NUMBER

This option uses a consecutive number for the invoices.
You can configure the current invoice number and the minimum length for the invoice number.
If the current invoice number is less than the minimum length, then the number is padded with leading 0s.
Here is an example. The current invoice number is 199 and the minimum length is set to 5.
Then the next invoice number would be: `00200`.

This format is always ongoing and is not reset at the end of the year!

### PREFIX - CONSEQUENTIAL NUMBER

This option corresponds to the format: `<PREFIX>-<CONSEQUENTIAL NUMBER>`.<br/>
For example: `RE-123`.<br/>
Here you can specify a prefix for the invoice number, the current number and the minimum length for the consecutive number.
The invoice number is not reset at the end of the year! With this format, the number always continues consecutively.

### CONSEQUENTIAL NUMBER/YEAR

This option corresponds to the format: `<CONSEQUENTIAL NUMBER>/<YEAR>`.<br/>
For example: `123/2025`.<br/>
The consecutive number is reset at the end of the year and the year is inserted at the end of the invoice number.
Invoices in the new year then start again with invoice number 1.
As with the first option, you can specify both the current number and the minimum length for the consecutive number.

### YEAR-CONSEQUENTIAL NUMBER

This option corresponds to the format: `<YEAR>-<CONSEQUENTIAL NUMBER>`.<br/>
For example: `2025-123`.<br/>
The year is inserted at the front of the invoice number, followed by a consecutive number.
The consecutive number is reset at the end of the year. Invoices in the new year then start again with invoice number 1.
As with the first option, you can specify both the current number and the minimum length for the consecutive number.

### YEAR MONTH DAY - DAY COUNTER

This option corresponds to the format: `<YEAR><MONTH><DAY>-<DAY COUNTER>`.<br/>
For example: `20250101-1`.<br/>
The invoice number consists of the year, month, day and a sequential day counter.
The day counter is reset every day. Invoices on the same day are then given the numbers 1, 2, 3, etc.
As with the first option, you can specify both the current number and the minimum length for the sequential number.

### YEAR MONTH - MONTHLY COUNTER

This option corresponds to the format: `<YY><MONTH>-<MONTHLY COUNTER>`.<br/> 
For example: `2501-1`.<br/>
The invoice number consists of the year, the month and a consecutive month counter.
The monthly counter is reset every month. Invoices in the same month are then given the numbers 1, 2, 3, etc.
As with the first option, you can specify both the current number and the minimum length for the consecutive number.

### PREFIX-YEAR-CONSEQUENTIAL-NUMBER

This option corresponds to the format: `<PREFIX>-<YEAR>-<CONSEQUENTIAL-NUMBER>`.<br/> 
For example: `RE-2025-123`.<br/>
Here you can specify a prefix for the invoice number, the current number and the minimum length for the consecutive number.
The year is always set automatically! The consecutive invoice number is reset at the end of the year!

### PREFIX-YY-CONSEQUENTIAL-NUMBER

This option corresponds to the format: `<PREFIX>-<YY>-<CONSEQUENTIAL-NUMBER>`.<br/> 
So, for example: `RE-25-123`.<br/>
Here you can specify a prefix for the invoice number, the current number and the minimum length for the consecutive number.
The year is always set automatically! The consecutive invoice number is reset at the end of the year!

### PREFIX-YYCONSEQUENTIAL-NUMBER

This option corresponds to the format: `<PREFIX>-<YY><CONSEQUENTIAL-NUMBER>`.<br/> 
So, for example: `RE-25123`.<br/>
Here you can specify a prefix for the invoice number, the current number and the minimum length for the consecutive number.
The year is always set automatically! The consecutive invoice number is reset at the end of the year!

## Credit note number

Here you can specify the format for the credit note number that should be used for credit notes.

## Bank details

Here you can store the bank details for your organization.
If you want to use the invoice module, you must store at least one bank account.
For customers, you can assign a different bank account to each customer.
When an outgoing invoice is sent to a customer, the bank details that you assigned to the customer are used
and displayed in the footer of the invoice.

## Logo

Here you can upload the logo for your organization.

You can upload a logo that will be used for all invoices and credit notes.
And you can upload a separate logo that will be displayed in the application.

## Margin calculation

Here you can set how the percentage margin should be calculated in the projects.

## Credit note strategy

Here you can set different strategies for the credit note process.

## Notifications

Here you can configure different email distribution lists for notifications.

There are various events in ZEIT.IO for which notifications can be sent.
For example, for submitted vacations, sick notes or for new incoming invoices.

## Holidays

Here you can configure the federal state for the holidays in the organization.
You can also enter additional holidays for the organization here.

## Data retention

Here you can set the data retention policy for your organization.
The data retention policy determines how long data is retained in ZEIT.IO.
After the deadline has expired, the data is automatically deleted!

You can currently set how long the working hours of permanent employees should be stored here.
This setting has no effect on the times of suppliers/freelancers.

A background job for the data retention policy is run once a day.
This background job deletes all data that is older than the specified deadline.
**Data that has been deleted once cannot be restored!**
If you set the value to 2 years, for example, all data that is older than 2 years will be deleted the next day at the latest.

## Main menu

Here you can configure which menu items should be displayed in the main menu.

## AddOns

Here you can activate AddOns for your organization.

## API Key

Here you can find the API key for your organization.
With this API key you can use the ZEIT.IO API and access your data programmatically.

## Audit logs

Here you can find the audit logs for your organization.
Here you can see who made which changes to the organization's settings and when.
