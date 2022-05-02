## Sending Messages to Groups (done by Marcel)

### Actor (User)
Faculty with a valid account in the system.

### Pre-conditions
Faculty is logged into the system. Information about all groups is already stored in the database.

### Main Flow
1. The faculty clicks on the **Groups** tab on the BTR490 website.
2. The system loads a list of all groups.
3. The faculty clicks on a **send message** hyperlink below a group's list of members.
4. The system brings up a model containing a form for the faculty to enter the email's subject and contents.
5. The faculty fills up both fields.
6. The faculty clicks on a **Submit** button to send the message to all students.
7. After the system succesfuly sends the message, the modal disapears.

### Alternate Flows
- If any connection issues arise, preventing the message to be sent before it times out: 
  1. The system will add an error message to the modal, warning the faculty that the message was not sent.
- If a faculty clicks on **Close**, instead of **Submit**:
  1. The modal disappears, and no further action is taken by the system. The contents of the modal will remain, though. Allowing the faculty to pick another group to send the message, for example.

### Postconditions
After a faculty has succesfully send a message, each member of the group (as well as the faculty) receives an email with its contents.
