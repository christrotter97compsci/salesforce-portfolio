# salesforce-portfolio

# How I adjusted the Organization-Wide Defaults
I went to "Sharing Setting" and adjusted the settings for the "Volunteer" and "Event" custom objects. I set both objects to Public Read Only for the Default Internal Access, but for the Default External Access, I set Event to "Public Read Only" and Volunteer to "Private" as those details are only internal.

# How I made the Role Hierarchy
I made two roles: Volunteer Manager and Working Volunteer. The "Volunteer Manager" reports to SVP Human Resources and "Working Volunteer" reports to the "Volunteer Manager"

# Two Sharing Rules Made
For the Event Object, I made a sharing rule called "Event Details." This rule contains the details of the event that is being coordinated and is shared with the Volunteer Manager.
For the Volunteer Object, I made a sharing rule called "How Event Task Completed." This rule shows how the volunteer completed task given to them at the event. It owned by the Working Volunteer and is shared with the Volunteer Manager.
