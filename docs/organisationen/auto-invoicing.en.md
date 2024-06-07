# Auto-Invoicing 

ZEIT.IO can automatically bill approved project times and expenses and also send the invoices automatically.
This saves you a lot of time and reduces errors.

## How does auto-invoicing work?

The auto-invoicing procedure is always linked to a project and must be explicitly activated in the project.
With this procedure, approved times and expenses from a specific period are automatically converted into an invoice 
and sent to the customer.

With this process, you can, for example, automatically convert an approved timesheet into an invoice and send it to the customer immediately after approval. 
Or you can use it to convert all approved times and expenses from the previous month into an invoice and send it on a scheduled basis on the Xth day of the month.

The auto-invoice procedure consists of the following components:

- **Trigger**: The trigger determines when the invoice is created and sent.
  There are event-based triggers and also time-based triggers. The trigger can be, for example,
  an approval or a specific day of the month.
- **Invoice type**: The invoice type determines what the invoice should look like.
- **Target state**: The target state determines whether the invoice should go into the draft or dispatch state.

## How do I configure the auto-outgoing invoice procedure?

You can always configure the auto-invoicing procedure in the project. 
This also means that you can have a different configuration for the auto-invoice procedure in each project. 
To do this, simply navigate to the project for which you want to configure the auto-invoicing procedure. 
In the bottom left of the page menu you will find the item "Auto-Invoicing". 
Here you can then make the settings for the auto-invoicing procedure.

## Auslöser konfigurieren

The trigger determines when the invoice should be created and sent.
There are event-based triggers and also time-controlled triggers.

### Event-based triggers

- **Timesheet approval**: The process is triggered when a timesheet is approved for the current project.
  The invoice created in this way contains all approved times from the timesheet.
  Regardless of the period over which the timesheet extends.
  Approved expenses from the same period and project are **not** included in the invoice.
  The invoice created in this way only contains the items in the approved timesheet.
- **Expenditure approval**: The process is triggered when an expense is approved for the current project.
  The invoice created in this way contains all approved expenses from the expense object.
  Regardless of the period over which the expense extends.
  Approved times from the same period and project are **not** included in the invoice.
  The invoice created in this way only contains the items from the approved expenses.
- **Timesheet OR expense approval**: The process is triggered when a timesheet **or** an expense is approved for the current project.
  The invoice created in this way only contains the items from the approved object.
  Regardless of the time period over which the time and expenses span.
  This trigger generates either an invoice for a timesheet or an invoice for an expense submission.

### Time-based triggers

- **The Xth day of the month**: The process is triggered on the Xth day of the month.
  The invoice created in this way contains all approved times and expenses from the previous month.
  The invoice contains all items that were approved in the previous month.
  The day of the month can be between 1 and 15.
- **Day X to Day Y of the month**: Every hour between the Xth and Yth day of the month, a check is made to see whether there are any approved times or expenses from the previous month that have not yet been billed.
  If this is the case, the items are billed.

## Configure invoice type

The invoice type determines how the invoice should look and what information it should contain. Currently, there are the following invoice types:

- **Project**: All booked times and expenses from the project are automatically added to the invoice.
  Expert names and project activities do not appear on this invoice.
- **Expert**: One invoice is generated for each expert. The project, name of the expert and the billing period appear on the invoice.
- **Experts**: One invoice is generated in which the hours are grouped by expert.
- **Activities**: One invoice is generated in which the hours are grouped by activity.
- **Maintenance contract - monthly:** A fixed maintenance fee is billed every month, which includes X service hours.
  Additional hours worked from the project that are not covered by the maintenance fee are also billed, if available.
- **Maintenance contract-Dacuro**: A fixed maintenance fee is billed every month, which includes X service hours.
  At the end of a quarter, additional hours worked on the project that are not covered by the maintenance fee are also billed.

## Configure target state

The target state is the state that the invoice should go into after it has been created.
The following states are possible:

- **Draft**: The invoice is created and transferred to the draft state. You can then check the invoice again and adjust it if necessary before sending it.
- **Completed**: The invoice is created and transferred to the completed state.
  You can then no longer edit the invoice. You can only send the invoice.
- **Completed and sent**: The invoice is created, completed and sent to the customer.
  You can then no longer edit the invoice.

You can also configure the language, date format and email recipient here, as well as how possible proof of performance should be attached to the invoice.
