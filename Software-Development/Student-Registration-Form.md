# 🧑‍🎓 Student Registration Form Application

## 📌 Overview

In this project, a Student Registration Form was created using Visual Studio and Visual Basic.

The application allows users to enter their details, validates the data, and confirms submission.

---

## 🎯 Purpose

- Collect user information
- Validate input
- Provide user-friendly interaction
- Simulate a registration system

---

## 📌 Tools & Technologies Used

- Visual Studio
- Visual Basic
- Windows Forms

---

## 📌 Controls Used

- **TextBox** → Name, email, phone
- **Label** → Field descriptions
- **Button** → Submit action
- **ComboBox** → Selection field
- **DateTimePicker** → Date of birth
- **Multiline TextBox** → Additional text input

---

## 📌 Form Design

The form included:
- Proper layout and alignment
- Increased font size
- Added colour and image
- Clear user-friendly structure

---

## 📌 Validation Implementation

### Empty Field Validation
- Fields cannot be left blank
- Error message displayed
- Textbox changes to red

### Date Validation
- Date of birth cannot be today’s date

---

## 💻 Sample Code (Validation Logic)

```vb
If TxtName.Text = "" Then
    MessageBox.Show("Name cannot be empty")
    TxtName.BackColor = Color.Red
End If

If DateTimePicker1.Value = Today Then
    MessageBox.Show("Date of Birth cannot be today's date")
End If
