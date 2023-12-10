# Ticketing system for city issues

This project aims to create a solution to the problem of issue communication between citizens and the city authorities.

## Description
The project is a system used for reporting, managing and browsing tickets describing city issues. The system consists of a web application and the backend.

### Web application
The purpose of the web application is to expose the backend's functionality to the users. This is the part that the user will directly interact with in the browser. This part

### Backend
The backend aims to provide the logical components, which will be connected to the web application. This is the part responsible for manipulating the database, processing data and requrest authorization.

## Functional requirements
### General
- the app allows browsing, creation, updating and deleting tickets.

### Tickets
- tickets can be filtered or sorted.
- tickets have to contain a description and be assigned to a  category.
- tickets can have additional data supplied, ex. image, location.
- created tickets cannot be modified after creation.
- comments can be added to a ticket for further communication.
- tickets can be rejected if they don't fulfill the requirements
- tickets can be marked as duplicate if they are describing the same underlying issue
- tickets can be forwarded to another worker or executor
- tickets can be marked as closed when the underlying issue is resolved

### User groups
- users can be assigned to any of the 3 different types: `BaseUser`, `OfficeWorker` or `Admin`
- the types are hierarchical, i.e. `OfficeWorker` can do everything an `BaseUser` can do and `Admin` can do everything `OfficeWorker` and `BaseUser` can do
- users can be `Individual` or `Group`
- application allows for browsing tickets without logging in
- application requires `BaseUser` privileges for ticket creation 
- `OfficeWorker` is responsible for taking further action with the ticket, i.e. forwarding, rejecting, marking as duplicate...
- `OfficeWorker` can change ticket status to one of the following: `New`, `In progress`, `Done`
- `Admin` can delete tickets
- `Admin` can assign privileges to other application operators

## Non-functional requirements:
- application can support 1000 users at the same time
- ticket creation time must not exceed 3 seconds
- each page of the web application should load in less than 2 seconds
- each ticket's ticket history is deleted automatically after 5 years 
- web application can be accessed from any of the mainstream web browsers - Firefox, Chrome, MS Edge and Safari
- the backend must have an uptime not lower than 95%
- the mean time to restore the system following a system failure must be less than 10 minutes
- database backup is created every day at 02:00 UTC
- application uses encrypted and secure HTTPS protocols

## Dictionary of terms

### General terms
- **Ticketing system, system**: this project as a whole, including the entirety of the hardware and software.
- **Ticket**: an entry for an issue that was reported.
- **User**: end client of this project, including the citizens and the city workers.
- **Comment**: a message attached to another piece of data, typically to a ticket.
- **Ticket category**: an abstract group the ticket is assigned to by the user, used for ease of searching
- **Executor** - person or company responsible for resolving the issue

### Ticket actions:
- **Ticket browsing**: examining reported issues on the platform.
- **Ticket creation**: the process of submitting detailed reports about city-releated problems or concerns.
- **Ticket rejection**: describes the act of denying further actions releated to this issue.
- **Mark as duplicate**: mark the ticket as describing the same issue as another ticket.
- **Ticket closure**: signalling that the underlying issue has been resolved.

## Ticket Forwarding and Closure:
- Redirecting reported issues to the appropriate personnel.
- Marking reported issues as resolved.


### Account Types:
- **BaseUser:** represents the default account level, mostly used for citizens.
- **OfficeWorker:** individuals responsible for managing and resolving reported issues.
- **Admin:** the highest-ranking person overseeing the entire system.

### User Categories:
- **Individual:** represents a single user.
- **Group:** denotes a collective of users working together.

### Technical terms
- **Web application**: the part of this project which will be present on end clients' devices, i.e. the graphical interface and communication logic.
- **Backend**: the central part of the code responsible for processing, validation, authorization and handling incoming actions
- **Frontend, user interface**: the part of the web application responsible for displaying information to the user.
- **Server** - the device used for executing core application code 
- **Database**: the part of this project responsible for data storage, including the tickets, user accounts, user privileges and other data.
- **Backup**: a copy of the database stored in case of unexpected events.