
<h2>Ticketing System</h2>
<p>Ticketing system web application for reporting, browsing, collecting city issues.</p>

<h3>Functional Requirements</h3>
<ul>
    <li>Has 3 Different types of users: [User, OfficeWorker, Admin]</li>
    <li>OfficeWorker inherits from User</li>
    <li>Admin inherits from OfficeWorker</li>
    <li>User can be Individual or Group</li>
    <li>Application allows for browsing tickets without logging in</li>
    <li>Tickets can be filtered or sorted</li>
    <li>Tickets can be filtered by: []</li>
    <li>Application allows for creating tickets with user privileges</li>
    <li>Creating ticket requires issue : description, category, image, location </li>
    <li>Issue category can be on of the following: []</li>    
    <li>Tickets cannot be modified</li>
    <li>Tickets can be commented</li>
    <li>Comments history is stored within tickets</li>
    <li>OfficeWorker gets tickets from Users</li>
    <li>OfficeWorker can change ticket status to one of the following: [New, In progress, Done]</li>    
    <li>OfficeWorker has additional capability to reject, duplicate, forward, close tickets</li>
    <li>Tickets can be rejected if they do not fulfill requirements</li>
    <li>Tickets can be duplicate if there is already a ticket that is redundant</li>
    <li>In case of wrong tickets assignment they can be forwarded</li>
    <li>Tickets can be closed when they are finished</li>
    <li>Admin can delete tickets</li>
    <li>Admin can assign privileges to other application operators</li>
</ul>

<h3>Non-Functional Requirements</h3>
<ul>
    <li>Application supports 1000 user at the same time</li>
    <li>Creating ticket time must be 3 second or less</li>
    <li>Page response time while refreshing must be lower than 2 seconds</li>
    <li>Maximum of 100 tickets can be listed on one site</li>
    <li>Ticket history is stored for 5 years</li>
    <li>Web application can be accessed from Linux or Windows operating system</li>
    <li>Application must perform without failure in 95 percent of use cases during a month</li>
    <li>The mean time to restore the system following a system failure must be less than 10 minutes</li>
    <li>Database Backup needs to be created at the end of each day</li>
    <li>All request are protected with sha256</li>
    <li>Application uses encrypted and secure HTTPS protocols</li>
</ul>

<h3>Hardware Requirements</h3>
<ul>
    <li>Server containing database approx. 100TB</li>
    <li>Server storage containing server backup approx. 100TB</li>
</ul>

<h3>Software Requirements</h3>
<ul>
    <li>Frontend: </li>
    <li>Backend: </li>
    <li>Database: </li>
    <li>Version control system: Git</li>
    <li>Software development platform: Github</li>
</ul>

