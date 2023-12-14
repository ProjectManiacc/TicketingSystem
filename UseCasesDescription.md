# Use Case Diagram Description

### Browse Tickets

- <b>Name:</b> Browse Tickets
- <b>Description:</b> Users can view a list of existing tickets in the system
- <b>Usual Scenario:</b> The user logs into the system, navigates to the "Browse tickets" 
functionality, and sees a list of available tickets 
- <b>Alternate Scenario:</b> The user attempts to browse tickets without logging in
- <b>Optional:</b>
    - <b>Trigger:</b> User navigates to the "Browse tickets"
    - <b>Preconditions:</b> None
    - <b>Postconditions:</b> The user can see and interact with the list of tickets

### Filter

- <b>Name:</b> Filter
- <b>Description:</b> Users can apply filters to customize the displayed list of tickets
- <b>Usual Scenario:</b> The user is on the "Browse tickets" page, accesses the "Filter" option, selects specific criteria, and applies the filter
- <b>Alternate Scenario:</b> The user attempts to apply a filter without being logged in
- <b>Optional:</b>
    - <b>Trigger:</b> User selects specific criteria and applies the filter
    - <b>Preconditions:</b> None
    - <b>Postconditions:</b> The list of tickets is updated based on the applied filter

### Sort

- <b>Name:</b> Sort
- <b>Description:</b> Users can sort the displayed list of tickets based on specific criteria
- <b>Usual Scenario:</b> The user is on the "Browse tickets" page, accesses the "Sort" option, selects a sorting criterion, and applies the sort
- <b>Alternate Scenario:</b> The user attempts to apply a sort without being logged in
- <b>Optional:</b>
    - <b>Trigger:</b> User selects specific criteria and applies the sort
    - <b>Preconditions:</b>
    - <b>Postconditions:</b> The list of tickets is reordered based on the selected sorting criterion

### Add Comment

- <b>Name:</b> Add Comment
- <b>Description:</b> Users can provide additional information or updates to existing tickets by adding comments
- <b>Usual Scenario:</b> The user logs into the system, selects a specific ticket, accesses the "Add comment" feature, and submits their comment
- <b>Alternate Scenario:</b> The user attempts to add a comment without being logged in
- <b>Optional:</b>
    - <b>Trigger:</b> The user selects "Add Comment" functionality
    - <b>Preconditions:</b> The user has successfully logged in and selected a ticket
    - <b>Postconditions:</b> The comment is added to the selected ticket

### Create Tickets

- <b>Name:</b> Create Tickets
- <b>Description:</b> Users initiates the process of creating a new ticket
- <b>Usual Scenario:</b> The user logs into the system, accesses the "Create ticket" feature, fills in necessary details, and submits the form
- <b>Alternate Scenario:</b> The user attempts to create a ticket without logging in
- <b>Optional:</b>
    - <b>Trigger:</b> The user selects "Create Ticket" functionality
    - <b>Preconditions:</b> The user has successfully logged in
    - <b>Postconditions:</b> A new ticket is created in the system

### Log in

- <b>Name:</b> Log in
- <b>Description:</b> Users must log in to access certain features and functionalities of the ticketing system
- <b>Usual Scenario:</b> The user navigates to the login page, enters valid credentials (email and password), and submits the login form
- <b>Alternate Scenario:</b> The user attempts to log in with invalid credentials
- <b>Optional:</b>
    - <b>Trigger:</b> User navigates to a page that requires authentication
    - <b>Preconditions:</b> The user is not logged in
    - <b>Postconditions:</b> The user is successfully authenticated and gains access to the protected features

### Reject Ticket

- <b>Name:</b> Reject Ticket
- <b>Description:</b> Office workers can reject a ticket that does not meet the criteria for resolution
- <b>Usual Scenario:</b> An office worker logs into the system, selects a ticket, and chooses the "Reject ticket" option
- <b>Alternate Scenario:</b> An office worker attempts to reject a ticket without logging in
- <b>Optional:</b>
    - <b>Trigger:</b> None
    - <b>Preconditions:</b> The office worker has successfully logged in and selected a ticket
    - <b>Postconditions:</b> The ticket is marked as rejected

### Mark as Duplicate

- <b>Name:</b> Mark as duplicate
- <b>Description:</b> Office worker can mark the ticket as duplicate if ticket is describing the same issue as another ticket
- <b>Usual Scenario:</b> An office worker logs into the system, selects a ticket, and chooses the "Mark as duplicate" option, specifying the related ticket
- <b>Alternate Scenario:</b> An office worker attempts to mark a ticket as a duplicate without selecting a related ticket
- <b>Optional:</b>
    - <b>Trigger:</b> None
    - <b>Preconditions:</b> The office worker has successfully logged in and selected a ticket
    - <b>Postconditions:</b> A ticket is being marked as duplicate

### Forward Ticket

- <b>Name:</b> Forward Ticket
- <b>Description:</b> Office workers can forward a ticket to another department or team for specialized handling
- <b>Usual Scenario:</b> An office worker logs into the system, selects a ticket, and uses the "Forward ticket" option to assign it to another team
- <b>Alternate Scenario:</b> An office worker attempts to forward a ticket without selecting delegated team
- <b>Optional:</b>
    - <b>Trigger:</b> None
    - <b>Preconditions:</b> Office worker has successfully logged in and selected a ticket
    - <b>Postconditions:</b> The ticket is reassigned to the specified team

### Close Ticket

- <b>Name:</b> Close Ticket
- <b>Description:</b> Office workers can mark a ticket as resolved and close the support case
- <b>Usual Scenario:</b> An office worker logs into the system, selects a ticket, and uses the "Close ticket" option
- <b>Alternate Scenario:</b> An office worker attempts to close a ticket without selecting one
- <b>Optional:</b>
    - <b>Trigger:</b> None
    - <b>Preconditions:</b> The office worker has successfully logged in and selected a ticket
    - <b>Postconditions:</b> The ticket is marked as closed

### Change Ticket Status

- <b>Name:</b> Ticket Status
- <b>Description:</b> Office workers can update the status of a ticket to reflect its current progress
- <b>Usual Scenario:</b> An office worker logs into the system, selects a ticket, and updates its status using the "Change ticket status" option
- <b>Alternate Scenario:</b> Office worker attemts to change the status from "new" directly to "close"
- <b>Optional:</b>
    - <b>Trigger:</b> None
    - <b>Preconditions:</b> The office worker has successfully logged in and selected a ticket
    - <b>Postconditions:</b> The ticket's status is modified accordingly

### Delete Ticket

- <b>Name:</b> Delete Ticket
- <b>Description:</b> Admins can permanently remove a ticket from the system
- <b>Usual Scenario:</b> An admin logs into the system, accesses the "Delete Ticket" feature, selects a ticket, and confirms the deletion
- <b>Alternate Scenario:</b> An admin attempts to delete ticket that is still "in progress"
- <b>Optional:</b>
    - <b>Trigger:</b> None
    - <b>Preconditions:</b> The Admin has successfully logged in and selected a ticket
    - <b>Postconditions:</b> The selected ticket is permanently removed from the system

### Assign Privileges 

- <b>Name:</b> Assign Privileges
- <b>Description:</b> Admins can grant specific privileges to others
- <b>Usual Scenario:</b> An admin logs into the system, accesses the "Assign Privileges" feature, selects an office worker or user, and assigns relevant privileges
- <b>Alternate Scenario:</b> An admin attempts to assign privileges to another admin
- <b>Optional:</b>
    - <b>Trigger:</b> None
    - <b>Preconditions:</b> The admin has successfully logged in and selected office worker or user
    - <b>Postconditions:</b> The selected office worker or user now has the assigned privileges
