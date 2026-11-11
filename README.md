# salesforce-portfolio

# How I adjusted the Organization-Wide Defaults
I went to "Sharing Setting" and adjusted the settings for the "Volunteer" and "Event" custom objects. I set both objects to Public Read Only for the Default Internal Access, but for the Default External Access, I set Event to "Public Read Only" and Volunteer to "Private" as those details are only internal.

# How I made the Role Hierarchy
I made two roles: Volunteer Manager and Working Volunteer. The "Volunteer Manager" reports to SVP Human Resources and "Working Volunteer" reports to the "Volunteer Manager"

# Two Sharing Rules Made
For the Event Object, I made a sharing rule called "Event Details." This rule contains the details of the event that is being coordinated and is shared with the Volunteer Manager.
For the Volunteer Object, I made a sharing rule called "How Event Task Completed." This rule shows how the volunteer completed task given to them at the event. It owned by the Working Volunteer and is shared with the Volunteer Manager.

# How I debugged a record-triggered flow
1. Deliberately broke the flow by changing the field value in the "Get The Coordinator" element to Create ID, which is the incorrect field.
2. Clicked Debug at the top, which brings up a debug panel on the left side of the screen.
3. Clicked Run at the bottom left after picking a record. Found out several things weren't going to work with this, so I had to rework the flow.
4. Added 3 new Get Record Elements, a Loop Element, and revised 2 an Update Record Element and Action Element
5. Created resource variable for the elements, which I didn't do last time.
6. When the Email action element wasn't working, I put in my own email address and it worked that way.
