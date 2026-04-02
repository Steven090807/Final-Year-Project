# 🎓 Student Assignment Management System 

<p align="left">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" />
  <img src="https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white" />
  <img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" />
</p>

<h4>A comprehensive, two-sided Learning Management System (LMS) built to bridge the gap between classroom administration and student engagement. This system features a dedicated Teacher Dashboard for content creation and a Student Portal for assignment tracking and submission.</h4>
<br>

## System Architecture: The Two-Sided Ecosystem

The application is engineered as a multi-user platform where data stays synchronized across two distinct interfaces:

### **1️⃣ The Teacher View (Administrative Control)**
* **Dynamic Classroom Creation:** Full CRUD (Create, Read, Update, Delete) capabilities for managing course modules.
* **Real-Time Note Management:** Implemented an **Inline Editing** system using JavaScript `contentEditable` and the Fetch API, allowing teachers to update syllabus notes without page refreshes.
* **Instructional Pipeline:** Advanced tools for posting study materials, setting deadlines with `due_datetime` logic, and uploading multi-format resources.
* **Relational Data Integrity:** Engineered with Referential Integrity logic. When a class is deleted, the system automatically triggers a cleanup of all associated student enrollments and assignments. This prevents "Orphaned Data" and ensures the database remains optimized and consistent.

### **2️⃣ The Student View (Task & Submission Engine)**
* **Join-Based Enrollment:** Securely connect to classes using unique class identifiers via a dedicated `check_class.php` validation layer.
* **Visual Status Indicators:** A logic-driven "Assignment Lifecycle" that uses color-coded feedback (e.g., Red for Assigned, Green for Submitted) to help students track progress.
* **Precision Countdown Engine:** A client-side JavaScript engine that provides second-by-second updates on deadlines, ensuring students never miss a submission.
* **Persistent UX:** Utilized `localStorage` to save user-specific UI preferences (like course card colors) to optimize frontend performance.
<br>

## 🛠️ Technical Implementation

### 1. Advanced Assignment Engine
* **Asynchronous Submissions:** Leverages the **Fetch API** and `FormData` objects for non-blocking file uploads, providing a smooth user experience.
* **Scalable File Metadata:** Engineered a solution to handle multiple attachments by encoding file paths into **JSON strings** within MySQL, reducing database complexity.

### 2. Security & Performance
* **Role-Based Access Control (RBAC):** Server-side PHP session validation ensures users can only access their respective views (Teacher vs. Student).
* **Database Integrity:** Implemented **SQL Prepared Statements** to prevent injection attacks and used input sanitization for all user-generated content.
* **Responsive Design:** Integrated **Bootstrap** with custom CSS breakpoints to ensure the LMS is fully functional on mobile and desktop.
<br>

## 🛠️ Technical Stack

| Layer | Technology |
| :--- | :--- |
| **Frontend** | HTML5, CSS3, Bootstrap, JavaScript |
| **Backend** | PHP (Object-Oriented) |
| **Database** | MySQL |
<br>

## 📝 Project Deliverables

- [x] **Fully Functional Web Application**
- [x] **Database Schema & Documentation**
- [x] **Technical Final Report & User Manual**
- [x] **Presentation Slides & Demo**
<br>

## Project Presentation Design (Teacher Interface)
<p align="center">
  <img src="IMG/Teacher_HomePage01.png">
  <br>
  <i>(Teacher Interface: Dashboard Home)</i>
</p>
<br><br>

<p align="center">
  <img src="IMG/Teacher_HomePage02.png">
  <br>
  <i>(Teacher Interface: Class Management / Add New Class)</i>
</p>
<br><br>

<p align="center">
  <img src="IMG/Teacher_AssPage01.png">
  <br>
  <i>(Teacher Interface: Assignment Overview)</i>
</p>
<br><br>

<p align="center">
  <img src="IMG/Teacher_AssPage02.png">
  <br>
  <i>(Teacher Interface: Create New Assignment)</i>
</p>
<br><br>

<p align="center">
  <img src="IMG/Teacher_AssPage03.png">
  <br>
  <i>(Teacher Interface: Assignment Guidelines)</i>
</p>
<br><br>

<p align="center">
  <img src="IMG/Teacher_AssPage04.png">
  <br>
  <i>(Teacher Interface: Assignment Guidelines)</i>
</p>
<br><br>

<p align="center">
  <img src="IMG/Teacher_AssPage05.png">
  <br>
  <i>(Teacher Interface: Student Submissions View)</i>
</p>
<br><br>

<p align="center">
  <img src="IMG/Teacher_UpdateAss01.png">
  <br>
  <i>(Teacher Interface: File Update & Management)</i>
</p>
<br><br>

<p align="center">
  <img src="IMG/Teacher_UpdateAss02.png">
  <br>
  <i>(Teacher Interface: View Assignment)</i>
</p>
<br><br>

<p align="center">
  <img src="IMG/Teacher_UpdateAss03.png">
  <br>
  <i>(Teacher Interface: Update File Function)</i>
</p>
<br><br>

<p align="center">
  <img src="IMG/Teacher_UpdateAss04.png">
  <br>
  <i>(Teacher Interface: Update File Function)</i>
</p>
<br><br>

<p align="center">
  <img src="IMG/Teacher_UpdateAss05.png">
  <br>
  <i>(Teacher Interface: Update File & View)</i>
</p>
<br><br>


<p align="center">
  <img src="IMG/Teacher_ClassPeople.png">
  <br>
  <i>(Teacher Interface: Class Members & Student List)</i>
</p>
<br><br>

## 👨‍🎓 Project Presentation Design (Student Interface)
<p align="center">
  <img src="IMG/Student_HomePage01.png">
  <br>
  <i>(Student Interface: Dashboard Home)</i>
</p>
<br><br>

<p align="center">
  <img src="IMG/Student_HomePage02.png">
  <br>
  <i>(Student Interface: Class Management / Join New Class)</i>
</p>
<br><br>

<p align="center">
  <img src="IMG/Student_HomePage03.png">
  <br>
  <i>(Student Interface: Class Search & Enrollment)</i>
</p>
<br><br>

<p align="center">
  <img src="IMG/Student_AssPage01.png">
  <br>
  <i>(Student Interface: Assignment Overview)</i>
</p>
<br><br>

<p align="center">
  <img src="IMG/Student_AssPage02.png">
  <br>
  <i>(Student Interface: Pending Assignment View)</i>
</p>
<br><br>

<p align="center">
  <img src="IMG/Student_AssPage03.png">
  <br>
  <i>(Student Interface: Completed Submission View)</i>
</p>
<br><br>

<p align="center">
  <img src="IMG/Student_ClassPage01.png">
  <br>
  <i>(Student Interface: Class Members & Student List)</i>
</p>
<br>

## Contact
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/steven0908)
[![Jobstreet](https://img.shields.io/badge/Jobstreet-003580?style=for-the-badge&logo=target&logoColor=white)](https://my.jobstreet.com/profiles/steven-gohyishen-97x9Q8tbmm)

> **Degree Final Year Project** &nbsp; | &nbsp; Completed on Nov 26, 2025  
> *Developed with passion for Software Engineering.*
