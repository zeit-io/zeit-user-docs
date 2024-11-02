# Outgoing invoices

You can create and send your invoices in the outgoing invoices section.
To do this, click on "Invoices" in the main menu and then on "Outgoing invoices".
There you will see a list of all invoices that have already been created.
New invoices can either be created manually, using the green "Create new invoice" button,
or automatically using the [Auto-invoicing feature](/organisationen/auto-invoicing.en/).

## Attachments

When you create an invoice, you can also add attachments. You can upload multiple PDF files
and these are then merged with the created invoice PDF. This means you receive a PDF invoice with
all the necessary attachments in a single file.

## Proof of performance (Timesheets)

If project times are billed with the invoice, then a proof of performance can optionally be selected
which contains the billed times. The proof of performance is then added as an attachment to the invoice.

There are various formats that you can choose for this proof of performance attachment:

### No proof of performance

With this option, no proof of performance is added to the invoice.

### Timesheet PDF attachment

If the invoice is of the type "Timesheet" (proof of performance) and the timesheet has a PDF attachment,
then the PDF from the timesheet is attached to the invoice. This option is particularly useful for
external proof of performance that was not created in ZEIT.IO. Read also
- [Get external performance proof approved](/freiberufler/leistungsnachweise.en/#have-external-proof-of-performance-approved).

### ZEIT.IO proof of performance (grouped by user)

The standard ZEIT.IO proof of performance is attached to the invoice. This contains a table with all approved time records for the selected period.
The entries include: 

 - date 
 - start & stop times 
 - project/activity 
 - comment 
 - name of the expert/user 
 - duration of the booking.

The time records are grouped by expert/user.
The performance records of the individual users are separated by page breaks.

### ZEIT.IO proof of performance (grouped by activity)

If activities are present, the first thing that is displayed is a table in which the booked times are grouped by activities.
A table with all approved time records for the selected period is then rendered. The entries include the date, start and stop times, project/activity, name of the expert/user, as well as comments and duration of the booking.

### Conti performance record

The Conti performance record is attached to the invoice.
This performance record complies with Continental Automotive's specifications.
DevUnits are used as the unit of measurement. 1 DevUnit = 1 hour. The DevUnits are grouped by activities.

### Dacuro performance record

This performance record contains a table with all approved time records for the selected period.
The entries include the date, project/activity, comments and duration of the booking.
Not included are start and stop times and the names of the experts/users.
If there are activities, the first thing that is displayed is a table in which the booked times are grouped by activities.
Since this performance record contains neither start nor stop times, entries with the same date and the same comment can be confusing. 
Therefore, entries with the same date and the same comment are summarized and the duration is added.

## CSV Export

Below the table on the right-hand side there is a link "CSV Export".
With this link you can download the current table for the outgoing invoices as a CSV file.

Each outgoing invoice is shown as a line in the CSV file.

The outgoing invoices can be filtered according to various criteria.
The CSV file contains the results of the current filter settings.

## DATEV CSV Export

If you filter the outgoing invoices according to a service month or year, an additional link "DATEV CSV Export" appears below the table on the right-hand side.
With this link you can download the current table for the outgoing invoices as a DATEV CSV file.
The DATEV CSV file contains all the outgoing invoices that were created in the selected service month or year.
Every single item on the outgoing invoice is shown as a line in the CSV file.
The file can therefore also contain more lines than the table on the website.

The file corresponds to the [DATEV booking stack format](https://developer.datev.de/datev/platform/de/dtvf/formate/buchungsstapel) and contains all the necessary information for accounting.
The DATEV CSV file can then be imported into your accounting software.

## FAQs

### Which email address are the invoices sent from?

By default, the invoices are sent from the email address `noreply@zeit.io`.
This email is also protected by SPF and DKIM.
The name of your organization always appears as the sender name. Like here, for example:

```
Muster-Organisations GmbH <noreply@zeit.io>
```

To ensure that the invoices reach the recipient, you should still inform the recipients
that you are using ZEIT.IO as your new invoice creation tool and that future invoices will come from the email address noreply@zeit.io.

### How can I cancel an invoice?

An invoice can only be canceled if it has not yet been paid.
To do this, click on the invoice you want to cancel and then on "Cancel" under "Actions" at the top right.
