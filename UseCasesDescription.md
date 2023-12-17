# Use Case Diagram Description

### Browse Tickets

- <b>Name:</b> Browse Tickets
- <b>Description:</b> Users can view a list of existing tickets in the system
- <b>Usual Scenario:</b> 
  - User logs into the system
  - Navigates to the "Browse tickets" functionality
  - Sees a list of available tickets 
  - <b>Optional:</b>
    - <b>Trigger:</b> User navigates to the "Browse tickets"
    - <b>Preconditions:</b> None
    - <b>Postconditions:</b> User can see and interact with the list of tickets
- <b>Alternate Scenario:</b> None

### Filter

- <b>Name:</b> Filter
- <b>Description:</b> Users can apply filters to customize the displayed list of tickets
- <b>Usual Scenario:</b> 
  - User is on the "Browse tickets" page 
  - Accesses the "Filter" option 
  - Selects specific criteria for filtering
  - Applies the filter
  - <b>Optional:</b>
     - <b>Trigger:</b> User selects specific criteria and applies the filter
     - <b>Preconditions:</b> User has successfully logged in and is on the "Browse tickets" page
     - <b>Postconditions:</b> The list of tickets is updated based on the applied filter
- <b>Alternate Scenario:</b> 
  - User is on the "Browse tickets" page 
  - Accesses the "Filter" option 
  - Attempts to apply the filter
  - <b>Optional:</b>
    - <b>Trigger:</b> User attempts to apply a filter without selecting any criteria
    - <b>Preconditions:</b> User has successfully logged in and is on the "Browse tickets" page
    - <b>Postconditions:</b>  The system displays an error message, prompting User to select valid filter criteria 

### Sort

- <b>Name:</b> Sort
- <b>Description:</b> Users can sort the displayed list of tickets based on specific criteria
- <b>Usual Scenario:</b> 
  - User is on the "Browse tickets" page 
  - Accesses the "Sort" option 
  - Selects specific criteria for sorting
  - Applies the sort
  - <b>Optional:</b>
      - <b>Trigger:</b> User selects specific criteria and applies the sort
      - <b>Preconditions:</b> User has successfully logged in and is on the "Browse tickets" page
      - <b>Postconditions:</b> The list of tickets is reordered based on the selected sorting criteria
- <b>Alternate Scenario:</b> 
  - User is on the "Browse tickets" page 
  - Accesses the "Sort" option 
  - Attempts to apply the sort
  - <b>Optional:</b>
    - <b>Trigger:</b> User attempts to apply a sort without selecting any criteria
    - <b>Preconditions:</b> User has successfully logged in and is on the "Browse tickets" page
    - <b>Postconditions:</b>  The system displays an error message, prompting User to select valid sort criteria
  

### Add Comment

- <b>Name:</b> Add Comment
- <b>Description:</b> Users can provide additional information or updates to existing tickets by adding comments
- <b>Usual Scenario:</b> 
  - User logs into the system
  - Selects his ticket
  - Accesses the "Add comment" feature
  - Submits their comment
  - <b>Optional:</b>
      - <b>Trigger:</b> User selects "Add Comment" functionality
      - <b>Preconditions:</b> User has successfully logged in and selected his ticket
      - <b>Postconditions:</b> The comment is added to the selected ticket
- <b>Alternate Scenario:</b>
  - User logs into the system
  - Selects ticket that does not belong to him
  - Attempts to add comment
  - <b>Optional:</b>
      - <b>Trigger:</b> User selects ticket, which does not belong to him
      - <b>Preconditions:</b> User has successfully logged in and selected his ticket
      - <b>Postconditions:</b> The system displays an error message, indicating that User cannot add comments to other user's tickets

### Create Tickets

- <b>Name:</b> Create Tickets
- <b>Description:</b> Users initiates the process of creating a new ticket
- <b>Usual Scenario:</b> 
  - User logs into the system
  - Accesses the "Create ticket" feature
  - Fills in necessary details: Description, Category, Image, Location
  - Submits the form
  - <b>Optional:</b>
      - <b>Trigger:</b> User selects "Create Ticket" functionality
      - <b>Preconditions:</b> User has successfully logged in
      - <b>Postconditions:</b> A new ticket is created in the system
- <b>Alternate Scenario:</b> 
  - User logs into the system
  - Accesses the "Create ticket" feature
  - Attempts to submit form with incomplete information
  - <b>Optional:</b>
      - <b>Trigger:</b> User selects option to submit ticket without filling all necessary details
      - <b>Preconditions:</b> User has successfully logged in
      - <b>Postconditions:</b> The system displays an error message, prompting User to provide all necessary details.

### Log in

- <b>Name:</b> Log in
- <b>Description:</b> Users must log in to access certain features and functionalities of the ticketing system
- <b>Usual Scenario:</b> 
  - User navigates to the login page
  - Enters valid credentials (email and password)
  - Submits the login form
  - <b>Optional:</b>
      - <b>Trigger:</b> User navigates to a page that requires authentication
      - <b>Preconditions:</b> User is not logged in
      - <b>Postconditions:</b> User is successfully authenticated and gains access to the protected features
- <b>Alternate Scenario:</b>
  - User navigates to the login page
  - Enters invalid credentials (email and password)
  - Attempts to submit the login form
  - <b>Optional:</b>
      - <b>Trigger:</b> User navigates to a page that requires authentication
      - <b>Preconditions:</b> User is not logged in
      - <b>Postconditions:</b>  The system displays an error message, prompting User to enter valid credentials

### Reject Ticket

- <b>Name:</b> Reject Ticket
- <b>Description:</b> Office workers can reject a ticket that does not meet the criteria for resolution
- <b>Usual Scenario:</b> 
  - An office worker logs into the system
  - Selects a ticket
  - Chooses the "Reject ticket" option
  - <b>Optional:</b>
      - <b>Trigger:</b> Office worker selects "Reject ticket" option
      - <b>Preconditions:</b> Office worker has successfully logged in and selected a ticket
      - <b>Postconditions:</b> The ticket is marked as rejected
- <b>Alternate Scenario:</b> 
  - An office worker logs into the system
  - Selects a ticket
  - Attempts to reject ticket with status "In progress"
  - <b>Optional:</b>
      - <b>Trigger:</b> Office worker selects "Reject ticket" option
      - <b>Preconditions:</b> Office worker has successfully logged in and selected a ticket
      - <b>Postconditions:</b> The system displays an error message, indicating that ongoing tickets cannot be rejected
      
### Mark as Duplicate

- <b>Name:</b> Mark as duplicate
- <b>Description:</b> Office worker can mark the ticket as duplicate if ticket is describing the same issue as another ticket
- <b>Usual Scenario:</b> 
  - An office worker logs into the system
  - Selects a ticket
  - Chooses the "Mark as duplicate" option, specifying the related ticket
  - <b>Optional:</b>
      - <b>Trigger:</b> Office worker selects "Mark as duplicate" option
      - <b>Preconditions:</b> Office worker has successfully logged in and selected a ticket
      - <b>Postconditions:</b> A ticket is being marked as duplicate
- <b>Alternate Scenario:</b> 
  - An office worker logs into the system
  - Selects a ticket
  - Attempts to choose the "Mark as duplicate" option without specifying the related ticket
  - <b>Optional:</b>
      - <b>Trigger:</b> Office worker selects "Mark as duplicate" option
      - <b>Preconditions:</b> Office worker has successfully logged in and selected a ticket
      - <b>Postconditions:</b> The system prompts Office worker to select a related ticket before marking the current ticket as a duplicate

### Forward Ticket

- <b>Name:</b> Forward Ticket
- <b>Description:</b> Office workers can forward a ticket to another department or team for specialized handling
- <b>Usual Scenario:</b> 
  - Office worker logs into the system
  - Selects a ticket
  - Chooses "Forward ticket" option to assign it to another team
  - <b>Optional:</b>
      - <b>Trigger:</b> Office worker selects "Forward ticket" option
      - <b>Preconditions:</b> Office worker has successfully logged in and selected a ticket
      - <b>Postconditions:</b> The ticket is reassigned to the specified team
- <b>Alternate Scenario:</b>
  - Office worker logs into the system
  - Selects a ticket
  - Attempts to choose "Forward ticket" option without selecting another team
  - <b>Optional:</b>
      - <b>Trigger:</b> Office worker selects "Forward ticket" option
      - <b>Preconditions:</b> Office worker has successfully logged in and selected a ticket
      - <b>Postconditions:</b> The system prompts Office worker to select a team before forwarding the ticket

### Close Ticket

- <b>Name:</b> Close Ticket
- <b>Description:</b> Office workers can mark a ticket as resolved and close the support case
- <b>Usual Scenario:</b> 
  - An office worker logs into the system
  - Selects a ticket
  - Chooses "Close ticket" option
  - <b>Optional:</b>
      - <b>Trigger:</b> Office worker selects "Close ticket" option
      - <b>Preconditions:</b> Office worker has successfully logged in and selected a ticket
      - <b>Postconditions:</b> The ticket is marked as closed
- <b>Alternate Scenario:</b> 
  - An office worker logs into the system
  - Selects a ticket
  - Attempts to choose "Close ticket" option for a ticket with status "New"
  - <b>Optional:</b>
      - <b>Trigger:</b> Office worker selects "Close ticket" option
      - <b>Preconditions:</b> Office worker has successfully logged in and selected a ticket
      - <b>Postconditions:</b> The system displays an error message, indicating that ticket that was not resolved cannot be closed

### Change Ticket Status

- <b>Name:</b> Ticket Status
- <b>Description:</b> Office workers can update the status of a ticket to reflect its current progress
- <b>Usual Scenario:</b> 
  - Office worker logs into the system
  - Selects a ticket
  - Modifies ticket status using the "Change ticket status" option
  - <b>Optional:</b>
      - <b>Trigger:</b> Office worker selects "Change ticket status" option
      - <b>Preconditions:</b> Office worker has successfully logged in and selected a ticket
      - <b>Postconditions:</b> The ticket's status is modified accordingly
- <b>Alternate Scenario:</b> 
  - Office worker logs into the system
  - Selects a ticket
  - Attempts to change ticket status from "New" to "Done", without previously selecting "In progress" option
  - <b>Optional:</b>
      - <b>Trigger:</b> Office worker selects "Change ticket status" option
      - <b>Preconditions:</b> Office worker has successfully logged in and selected a ticket
      - <b>Postconditions:</b> The system displays an error message, indicating that ticket status has to be modified in an order "New" -> "In progress" -> "Done"

### Delete Ticket

- <b>Name:</b> Delete Ticket
- <b>Description:</b> Admins can permanently remove a ticket from the system
- <b>Usual Scenario:</b> 
  - An admin logs into the system
  - Accesses the "Delete Ticket" feature
  - Selects a ticket
  - Confirms the deletion
  - <b>Optional:</b>
      - <b>Trigger:</b> Admin selects "Delete ticket" option
      - <b>Preconditions:</b> Admin has successfully logged in and selected a ticket
      - <b>Postconditions:</b> The selected ticket is permanently removed from the system
- <b>Alternate Scenario:</b>
  - An admin logs into the system
  - Accesses the "Delete Ticket" feature
  - Selects a ticket
  - Attempts to delete ticket with status "In progress"
  - <b>Optional:</b>
      - <b>Trigger:</b> Admin selects "Delete ticket" option
      - <b>Preconditions:</b> Admin has successfully logged in and selected a ticket
      - <b>Postconditions:</b> The system displays an error message, indicating that ongoing tickets cannot be deleted
    
### Assign Privileges 

- <b>Name:</b> Assign Privileges
- <b>Description:</b> Admins can grant specific privileges to others
- <b>Usual Scenario:</b> 
  - Admin logs into the system
  - Accesses the "Assign Privileges" feature
  - Selects an office worker or user
  - Assigns relevant privileges
  - <b>Optional:</b>
      - <b>Trigger:</b> Admin selects "Assign privileges" option
      - <b>Preconditions:</b> Admin has successfully logged in and selected office worker or user
      - <b>Postconditions:</b> The selected office worker or user now has the assigned privileges
- <b>Alternate Scenario:</b>
  - Admin logs into the system
  - Accesses the "Assign Privileges" feature
  - Selects another admin
  - Attempts to assign relevant privileges
  - <b>Optional:</b>
      - <b>Trigger:</b> Admin selects "Assign privileges" option
      - <b>Preconditions:</b> Admin has successfully logged in and selected another admin
      - <b>Postconditions:</b> The system displays an error message, indicating that admins cannot assign privileges to other admins