# Projects 

Projects are a central part of ZEIT.IO!
Each project has a unique identifier, a name, a start and end date, an hourly budget and a currency budget.
Times (TimeRecords), expenses and fixed price packages can be booked to projects.
Projects that belong to an organization can be edited by multiple people.
Each project has a member list that lists all people who are allowed to book on the project.
In addition, each project also has an approval list that lists all people who are allowed to approve bookings on the project.

If you are in the context of the organization, you will find the item "Projects" in the main menu.
Here you can see all the projects that belong to the organization.
And you can also create new projects.

## Name vs. Identifier

Every project has a name and an identifier. These are identical by default, but can also be different.
The name of the project is relevant for the invoice module.
The name is used on invoices and credit notes.
Set the project name accordingly as you want the project to be represented on outgoing invoices and credit notes.

The project identifier must be unique within the organization and is used within the application
to display the project. For example, the project identifier is always displayed in the project selection for time recording.
And when recording expenses, the project identifier is always displayed in the project selection. Not the name!

Both the name and the identifier can be changed at any time.

## Project Description

Every project can have a description. The description is optional and can be changed at any time.
The description is visible to project members and project approvers and can be used to provide additional information about the project.

## Project period

Every project has a start and end date.
All bookings (times, expenses, fixed price packages) must be within the project period.
Bookings that are outside the project period cannot be booked to the project.
Start and end dates can be changed at any time.

## Budgets

A project always has an hourly budget and a total currency budget.
The hourly budget is the maximum number of hours that can be booked to the project.
The total currency budget is the amount available for the project.
The total currency budget is the sum of the following three budgets:

- **Budget (time tracking)**: The currency budget for time tracking.
- **Budget (expenses)**: The currency budget for expenses.
- **Budget (fixed price packages)**: The currency budget for the fixed price packages.

By default, ZEIT.IO also ensures that these budgets are not exceeded.
Unless the option for "Allow overbookings" is activated.
In that case, the budgets can also be exceeded.

## Project number & order number

Projects can optionally have a project number and an order number.
In the organization settings, you can configure whether these fields should be mandatory or not.
By default, these fields are not mandatory.

If a project number or order number is stored, then this will also be used on outgoing invoices and credit notes.
In addition, the following elements can also be filtered by project number and/or order number:

- Times (TimeRecords)
- Expenses/travel costs
- Proof of performance (timesheets)
- Outgoing invoices
- Incoming invoices
- Credit notes

## Interval

The interval in the project can be used to configure how finely granular the time recording should be.
By default, time recording in the project is accurate to the minute.
However, different intervals can also be configured, such as 5 minutes, 10 minutes, 15 minutes or 30 minutes.
In this case, time recording is always rounded to the next interval.
So that all booked times can be evenly divided by an interval.

If, for example, a 10-minute interval is configured, then a time of 12 minutes is rounded up to 20 minutes.
Every interval started is therefore always billed in full.

## Customer

Each project can optionally be assigned to a customer.
The dropdown for customer selection not only shows the customers, but also the customer's stored departments and contact persons.
Ideally, you assign the project to the right department or contact person who is responsible for receiving the invoice.

If project times or expenses are billed, the invoice module is pre-filled with the customer who is assigned to the project.

In addition, projects, times, expenses and proof of performance can then also be filtered by customer.

## Contact person

Every project can optionally have a contact person.
The contact person is visible to all project members and project approvers.
The contact person can be used to store a contact person for the project.

## Dynamic fields

Projects can optionally have dynamic fields.
If you want to store certain information about the project that is not shown in the standard fields, you can do this with dynamic fields.
Dynamic fields always consist of a key-value pair. This is the identifier and the value is the content.

The dynamic fields from the project are automatically transferred to outgoing invoices and appear on the top right of the outgoing invoices.
If your customer wants to see other numbers on the invoice in addition to the project number and order number, e.g. a very specific SAP number, you can do this with dynamic fields.

The dynamic fields are **not** transferred to credit notes.
The dynamic fields are only transferred to outgoing invoices!

Dynamic fields are not visible to project members and project approvers.
These fields are only visible to people who have read access to projects and the organization's billing module.
Dynamic fields can be added, changed or deleted at any time.

## Comments in time tracking mandatory

Projects can optionally be configured to require a comment when tracking time.
This is also the default setting.

## Billable

Projects can be configured to be billable.
This means that time, expenses and fixed price packages booked to the project can also be billed.
If a project is not billable, then time, expenses and fixed price packages booked to the project cannot be billed.
Projects that are not billable do not appear in the billing module either.

The default setting is that projects are billable.
