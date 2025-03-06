# Student Verification System

## Overview
The **Student Verification System** ensures that student cards are only issued to **registered** students. It achieves this by validating student details against the university’s database before approving card issuance.

### **Problem Statement**
Currently, the university issues student cards without verifying the student's registration status, allowing unauthorized individuals to create fake student cards. This system will prevent that by:
- Checking student details against the university’s database.
- Approving or denying student card requests based on registration status.
- Providing logs for audit purposes.

---

## **System Architecture**
This system consists of:
1. **User Input Module:** Accepts student details.
2. **Database Interface:** Connects to the university's database.
3. **Verification Logic:** Confirms student registration.
4. **Response Handling:** Grants or denies card issuance.

---

## **Requirements**
### **Software Requirements**
- **Operating System:** Linux/macOS/Windows
- **Programming Language:** C++/ Python
- **Database:** MySQL or PostgreSQL (for university data)
- **Build System:** CMake or Makefile

### **Hardware Requirements**
- At least **4GB RAM** (for smooth database operations)
- At least **50MB disk space** for logs and database storage

---

## **Database Setup**
### **1. Database Schema**
The university database should contain a `students` table structured as follows:

```sql
CREATE TABLE students (
    student_id VARCHAR(20) PRIMARY KEY,
    first_name VARCHAR(50),
    last_name VARCHAR(50),
    date_of_birth DATE,
    department VARCHAR(100),
    year_of_study INT,
    registration_status BOOLEAN
);



<!---
Thobile378/Thobile378 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
