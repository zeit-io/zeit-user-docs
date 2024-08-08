# Projects

Projects are a central part of ZEIT.IO!
Every project has a unique identifier, a name, a start and end date, an hourly budget and a currency budget.
Times (TimeRecords), expenses and fixed price packages can be booked to projects.
Projects that belong to an organization can be edited by multiple people.
Every project has a member list that lists all people who are allowed to book on the project.
In addition, every project also has an approval list that lists all people who are allowed to approve bookings on the project.

If you are in the context of the organization, you will find the item "Projects" in the main menu.
Here you can see all the projects that belong to the organization.

## Create a new project

If you click on "Projects" in the main menu, you will see a list of all the projects you have access to.
At the top right of the page there is a button "Create new project". 
If you click on it, a dialog box opens in which you can create a new project.

## Project fields

If you create a new project or edit an existing project, a form with various fields opens.
All fields are explained in detail below.

### Project type

There are currently two project types at ZEIT.IO: "Time & Material" and "Fixed price".
The project type determines how the margin is calculated in the project.

#### Time & Material

With the "Time & Material" project type, the project is billed according to the effort involved.
For these projects, an hourly rate or daily rate has been agreed with the customer and the effort incurred is billed accordingly.

For Time & Material projects, the margin is always 0 at the start of the project.
Because no effort has been booked yet, there is no margin.

The margin is calculated based on the times booked.
The members of the project have all assigned an purchase- and a sales hourly rate. 
The difference between the sales and purchase hourly rate is the margin.

Here is an example. 
The freelancer Max Mustermann is registered as a member in the project and the following hourly rates are assigned in his project membership:

- Sales hourly rate: €100
- Purchase hourly rate: €77

The margin per hour is therefore €23. 
If he books two hours on the project, the margin in the project is €46.

The margin in the project increases with each booked time.

#### Fixed price

With the project type "fixed price", the project is billed at a fixed price.
Here we assume that the currency budget stored for the project is also the fixed price.

If the project has a currency budget of €100,000, then that is also the fixed price at which the project is billed.
Regardless of how many hours are booked.

For the margin calculation, this means that the margin in the project is always 100% at the beginning.
The full currency budget is always shown as the margin at the beginning. 
For example, €100,000.
Because no expenses have been incurred yet.
If expenses are then booked in the project, the margin drops accordingly.

Here is an example. 
The freelancer Max Mustermann is registered as a member in the project and the following hourly rates are stored in his project membership:

- Sales hourly rate: €100
- Purchase hourly rate: €77

As this is a fixed-price project, the stored sales hourly rate is irrelevant for the margin calculation.
In this case, only the purchase hourly rate is relevant.
If Max now books two hours on the project, he incurs costs worth €154.
The margin in the project accordingly drops from €100,000 to €99,846.
Every booked time and every booked expense reduces the margin in the project.

### Name vs. Identifier

Every project has a name and an identifier. These are identical by default, but can also be different.
The name of the project is relevant for the invoice module.
The name is used on invoices and credit notes.
Set the project name accordingly as you want the project to be represented on outgoing invoices and credit notes.

The project identifier must be unique within the organization and is used within the application
to display the project. For example, the project identifier is always displayed in the project selection for time recording.
And when recording expenses, the project identifier is always displayed in the project selection. Not the name!

Both the name and the identifier can be changed at any time.

### Project Description

Every project can have a description. The description is optional and can be changed at any time.
The description is visible to project members and project approvers and can be used to provide additional information about the project.

### Project period

Every project has a start and end date.
All bookings (times, expenses, fixed price packages) must be within the project period.
Bookings that are outside the project period cannot be booked to the project.
Start and end dates can be changed at any time.

### Budgets

Projects on ZEIT.IO have the following budgets:

- **Hourly budget**: The maximum number of hours that can be booked on the project.
- **Budget (time tracking)**: The currency budget for time tracking. This sum is usually the hourly budget multiplied by the average hourly sales rate.
- **Budget (expenses)**: The currency budget for expenses/travel costs.
- **Budget (fixed price packages)**: The currency budget for fixed price packages.
- **Budget (total)**: The sum of the three currency budgets (time tracking, expenses, fixed price packages).

By default, ZEIT.IO ensures that these budgets are adhered to.
If a booking would exceed one of the budgets, the booking will be rejected.
Unless the option for "Allow overbookings" is activated.
In this case, the budgets can also be exceeded.

!!! Info
    If times are to be booked to the project, then the hourly budget and budget (time recording) must be stored.
    In this case, both fields must be greater than 0. If one of the two fields is 0, then no times can be booked to the project!

### Project number & order number

Projects can optionally have a project number and an order number.

In the organization settings, under the item "General", you can configure the order number to be a mandatory field.
If this option is activated, an order number must be entered when creating a new project!
This has no effect on existing projects.
The same option is also available for the project number.
The project number can also be configured as a mandatory field.

However, these fields are not mandatory by default.

If a project number or order number is entered, this is also used on outgoing invoices and credit notes.
In addition, objects assigned to the project can also be filtered by project number and/or order number.
This includes the following objects:

- Times (TimeRecords)
- Expenses/travel costs
- Proof of work (timesheets)
- Outgoing invoices
- Incoming invoices
- Credit notes

If the order number/project number is changed in the project, the change is also applied to all of the objects mentioned above.
This ensures that filtering by project number/order number is always correct.

### Interval

The interval in the project can be used to configure how finely granular the time recording should be.
By default, time recording in the project is accurate to the minute.
However, different intervals can also be configured, such as 5 minutes, 10 minutes, 15 minutes or 30 minutes.
In this case, time recording is always rounded to the next interval.
So that all booked times can be evenly divided by an interval.

If, for example, a 10-minute interval is configured, then a time of 12 minutes is rounded up to 20 minutes.
Every interval started is therefore always billed in full.

### Customer

Each project can optionally be assigned to a customer.
The dropdown for customer selection not only shows the customers, but also the customer's stored departments and contact persons.
Ideally, you assign the project to the right department or contact person who is responsible for receiving the invoice.

If project times or expenses are billed, the invoice module is pre-filled with the customer who is assigned to the project.

In addition, projects, times, expenses and proof of performance can then also be filtered by customer.

### Contact person

Every project can optionally have a contact person.
The contact person is visible to all project members and project approvers.
The contact person can be used to store a contact person for the project.

### Dynamic fields

Projects can optionally have dynamic fields.
If you want to store certain information about the project that is not shown in the standard fields, you can do this with dynamic fields.
Dynamic fields always consist of a key-value pair.
Where the "key" is the identifier and the "value" is the content.

The dynamic fields from the project are automatically transferred to outgoing invoices and appear on the top right of the outgoing invoices.
If your customer wants to see other numbers on the invoice in addition to the project number and order number, e.g. a very specific SAP number, you can do this with dynamic fields.

The dynamic fields are **not** transferred to credit notes.
The dynamic fields are only transferred to outgoing invoices!

Dynamic fields are not visible to project members and project approvers.
These fields are only visible to people who have read access to projects and the organization's billing module.
Dynamic fields can be added, changed or deleted at any time.

### Comments in time tracking mandatory

Projects can optionally be configured to require a comment when tracking time.
This is also the default setting.

### Billable

Projects can be configured to be billable.
This means that time, expenses and fixed price packages booked to the project can also be billed.
If a project is not billable, then time, expenses and fixed price packages booked to the project cannot be billed.
Projects that are not billable do not appear in the billing module either.

The default setting is that projects are billable.

### Overbookable

Projects can optionally be configured to allow overbookings.
By default, overbookings are not allowed and ZEIT.IO ensures that all budgets are adhered to.
If a booking exceeds the hourly budget or one of the currency budgets, the booking is rejected.
However, if the checkbox for "Allow overbookings" is activated, the budgets can also be exceeded.
