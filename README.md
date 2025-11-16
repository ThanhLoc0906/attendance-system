# Student Attendance System

A desktop-based **Student Attendance Management System** built with **Python (Tkinter)** and **SQLite**.
The application supports three user roles (Admin, Teacher, Student) and provides simple interfaces for taking attendance, viewing history, generating reports, and managing accounts/courses/classes.

---

## 🚀 Features

- **User Login & Role-based Access**
  - Admin, Teacher, and Student roles
  - Error message for invalid username/password
- **Teacher Dashboard**
  - Add attendance records (Student ID, Name, Status, Date)
  - Validation for missing fields
  - Refresh and **Reset All** attendance
  - View history & summary report
  - Update profile (change password)
- **Student Dashboard**
  - View their own attendance history
  - Cannot see or use the Reset All button
  - Update profile (change password)
- **Admin Dashboard**
  - Manage user accounts (add/delete users and roles)
  - Manage courses
  - Manage classes linked to courses
- **Password Functions**
  - Reset Password from Login screen
  - Update Profile while logged in
- **Reporting**
  - Attendance summary per student (Total, Present, Absent, Late)

---

## 🛠 Tech Stack

- **Language:** Python 3.x  
- **GUI:** Tkinter (with `ttk` widgets)  
- **Database:** SQLite (`attendance_gui.db`)  
- **Images:** Pillow (PIL) for loading the university logo  

---

## 📂 Project Structure

```text
attendance-system/
├── attendance_gui.py            # Main application file (GUI + logic)
├── attendance_gui.db            # SQLite database
├── uth.png                      # University logo displayed in the UI
├── project_full_report.docx     # Project report (requirements, design, testing)
├── Stage4_Testing_Formatted.docx# Detailed Stage 4 – Testing document
├── test_cases_template_10_numbered.xlsx   # 10 core test cases (official template)
└── README.md
```

You may not have all of these files in your copy, but this is the recommended structure for the final project submission.

---

## ▶ How to Run

1. Make sure you have **Python 3.x** installed.
2. Install required libraries (if not already available):

   ```bash
   pip install pillow
   ```

3. Place `attendance_gui.py`, `attendance_gui.db`, and `uth.png` in the same folder.
4. Run the application:

   ```bash
   python attendance_gui.py
   ```

---

## 🔑 Default Test Accounts

You can use the following accounts for testing (example):

- **Teacher**  
  - Username: `teacher`  
  - Password: `1234`
- **Student**  
  - Username: `student`  
  - Password: `0000`
- **Admin** (if implemented)  
  - Username: `admin`  
  - Password: `admin`

> You can change or add more accounts through the **Admin Dashboard** or directly in the `users` table inside `attendance_gui.db`.

---

## ✅ Testing

Testing was performed using a set of **10 core test cases** designed with the official **“Testing Document Template”**:

- Test Case 1 – Successful login (teacher)
- Test Case 2 – Wrong password (error message)
- Test Case 3 – Save valid attendance
- Test Case 4 – Validation for missing Student ID
- Test Case 5 – Reset All (teacher confirms YES)
- Test Case 6 – Student cannot see the Reset All button
- Test Case 7 – Reset Password for an existing user
- Test Case 8 – Update Profile (change password)
- Test Case 9 – Attendance summary report per student
- Test Case 10 – Admin adds a new account and login is successful

Details are documented in:

- `Stage4_Testing_Formatted.docx`  
- `test_cases_template_10_numbered.xlsx`

---

## 📸 Screenshots (optional)

You can add screenshots such as:

- Login screen  
- Teacher Dashboard  
- Student Dashboard  
- Admin Dashboard  
- Sample report / history window  

Create a folder `screenshots/` and upload the images there, then reference them in this README.

---

## 📚 Future Improvements

- Export attendance reports to Excel or PDF  
- Add search & filter by date range and class/course  
- Implement authentication security improvements (password hashing, etc.)  
- Convert to a web application (Django/Flask) or mobile app  

---

## 👤 Author

- **Student:** (Nguyễn Thành Lộc)  
- **GitHub:** [ThanhLoc0906](https://github.com/ThanhLoc0906)

Feel free to fork, modify, or improve this project for learning and academic purposes.
