## Picking a Timeslot (done by Marcel)

### Actor (User)
Student with a valid account in the system and an assigned CAPSTONE group.

### Pre-conditions
Student is logged into the system. No other student from the same CAPSTONE group has already picked a timeslot for the group.

### Main Flow
1. The student clicks on the **Meetings** tab on the BTR490 website.
2. The system loads a list of meeting timeslots.
3. The students clicks on an available timeslot.
4. The system asks the student to confirm his/her choice.
5. After the student confirms his/her choice, the system reloads the page and displays that the chosen timeslot belongs to the student's group.
6. The system sends an email to all members of the group.

### Alternate Flows
- If another student from the same group has already picked a timeslot:
  1. After step 3, the system will let the student know that his/her group already has an assigned timeslot.
- If a student clicks on a timeslot that has already been picked:
  1. After step 3, the system will let the student know that the chosen timeslot is already taken. The system will allow the user to chose another timeslot, effectively sending him/her back to step 2.
- If a student does not confirm his/her choice:
  1. After step 4, the system will allow the user to chose another timeslot, effectively sending him/her back to step 2.

### Postconditions
After a student has succesfully picked a timeslot, the database gets updated with the information about which group has picked which timeslot. Moreover, each member of the group (as well as the faculty) receives an email with all information about the meeting.
