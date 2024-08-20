# Admin Page for Online Teaching Site

This frontend is designed to manage the organization's database for an online teaching site. It interacts with the backend API to handle various operations related to students and mentors.

## Visit

Check out the live demo: [Admin Page](https://httdbadminpage.netlify.app/)

## API URL

This frontend communicates with the following API: [Backend API](https://assign-mentor-rwbp.onrender.com)

## API Documentation

You can explore the API in Postman: [View Documentation](https://documenter.getpostman.com/view/34103499/2sA3XWdycy)

## Features and Operations

### `/students`

- Displays all students in the database.

### `/mentors`

- Displays all mentors in the database.

### `/addmentor`

- Allows adding a new mentor to the database.

### `/addstudent`

- Allows adding a new student to the database.

### **Assigning Students to a Mentor**  
**`/assignstudent/:MentorID`**

1. Add students to a mentor based on course proficiency.
2. Excludes students already assigned to a mentor.

### **Changing Mentor for a Student**  
**`/changementor/:studentID`**

1. Change the mentor for a particular student by providing a new mentor ID.
2. The existing mentor ID is replaced with the new one, and the old mentor ID is pushed into the student's previous mentor information.

### **Displaying Students for a Particular Mentor**  
**`/displaystudents/:mentorID`**

1. Displays students assigned to a specific mentor by matching the mentor ID in the student database.

### **Display Students Previously Assigned to a Mentor**  
**`/previousmentor/:studentID`**

1. Displays the previous mentors assigned to a particular student.

---

This admin page provides an easy-to-use interface for managing students and mentors within the organization's database, ensuring a seamless workflow for the online teaching site.
