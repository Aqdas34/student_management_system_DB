# **Student Management System – Oracle Database Backend**  

## **Overview**  
The **Student Management System** is a **comprehensive academic administration software** designed to manage faculty, students, academic programs, courses, and classroom operations. Built on an **Oracle Database**, it ensures efficient data organization and retrieval for academic institutions.  

## **Key Features**  

### **📌 Faculty & Department Management**  
- **Faculty Table:** Stores faculty details, including **Faculty_ID** and **Faculty Name (F_name)**.  
- **Department Table:** Maintains departments linked to faculties using **Foreign Keys (Facult_ID, dept_ID)**.  

### **🎓 Academic Roles & Members**  
- **Member Table:** Captures all academic and non-academic members.  
- **TEACHING & NON_TEACHING Tables:** Define academic and administrative roles as subtypes.  

### **📚 Degree Programs & Student Records**  
- **DEGREE_PROGRAMS Table:** Stores degree details, including **degree_ID, program name**, and supervisor (TMem_ID).  
- **STUDENT Table:** Maintains student information such as **roll number (rollNo), name, date of birth, contact details, and department association**.  

### **📖 Course Management**  
- **COURSES Table:** Contains **course codes (C_Code), titles, and credit hours**.  
- **PRE_COURSE Table:** Manages course prerequisites.  
- **DEGREE_COURSES Table:** Defines **many-to-many relationships** between degrees and courses.  

### **🏫 Classroom & Academic Operations**  
- **ROOM, CLASSROOM, and LAB Tables:** Manage room allocations for lectures and labs.  
- **SECTION Table:** Handles course sections and student enrollment.  
- **SECTION_ENROLLMENT & SECTION_WITHDRAW Tables:** Track student enrollments and withdrawals.  
- **SECTION_ATTENDANCE Table:** Stores student attendance records.  

## **Technology Stack**  
- **Database:** Oracle Database  
- **Programming Language:** SQL (PL/SQL for stored procedures & triggers)  
- **Schema Design:** Normalized relational structure for efficient querying  
