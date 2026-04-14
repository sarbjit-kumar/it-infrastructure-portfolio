# 🖥️ Multi-Form Application (Course Registration System)

## 📌 Overview

In this project, a multi-form Windows application was developed using Visual Studio and Visual Basic.

The application includes:
- Main Front Page
- Login Form
- Apply for a Course Form
- Contact Us Form

---

## 🎯 Purpose

- Provide a user-friendly interface
- Allow navigation between multiple forms
- Collect and validate user information
- Simulate a real-world application

---

## 📌 Tools & Technologies Used

- Visual Studio
- Visual Basic
- Windows Forms

---

## 📌 Application Structure

### 🔹 Main Front Page
Contains three buttons:
- Login Account
- Apply for a Course
- Contact Us

### 🔹 Login Form
Contains:
- Username
- Password
- Submit button

### 🔹 Apply for a Course Form
Contains:
- First Name
- Last Name
- Gender
- Date of Birth
- Email Address
- Mobile Number
- Landline Number
- Course Selection and Price
- Submit button

### 🔹 Contact Us Form
Contains:
- Email Address
- Query
- Submit Query button

---

## 📌 Navigation Logic

Each form is connected using button click events.

### 💻 Example Code

```vb
ApplyForm.Show()
Me.Hide()
```

---

## 📌 Validation Implementation


### Empty Field Validation

```vb
If TxtUsername.Text = "" Or TxtPassword.Text = "" Then
    MessageBox.Show("Fields cannot be empty")
End If
```

---
