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

### Email Validation

```vb
If Not TxtEmail.Text.Contains("@") Then
    MessageBox.Show("Invalid Email Format")
End If
```

---

### Mobile Number Validation

```vb
If TxtMobile.Text.Length < 9 Then
    MessageBox.Show("Invalid Mobile Number")
End If
```

---

## 📌 User Testing

User testing confirmed:

- Submit buttons worked on all forms  
- Validation messages displayed correctly  
- Navigation worked correctly  

---

## 🐞 Debugging

Debugging was performed using breakpoints:

- Breakpoints were added in validation code  
- Step-by-step execution helped identify issues  

---

## 🧪 Black Box Testing

Example test cases:

| Test Case     | Input        | Expected Output        |
|--------------|-------------|----------------------|
| Empty fields | No input    | Error message        |
| Invalid email| wrongformat | Validation error     |
| Valid input  | correct data| Successful submission|

---

## 📊 Application Analysis

### 🔹 Strengths

- User-friendly design  
- Multiple form navigation  
- Validations implemented  

---

### 🔹 Limitations

- No database integration  
- Basic validations only  

---

### 🔹 Recommendations

- Add database support  
- Improve UI design  
- Add advanced validations  

---

## 📌 Key Concepts Demonstrated

- Multi-form design  
- Navigation logic  
- Event-driven programming  
- Validation  
- Debugging and testing  

---

## 📌 Real-world Relevance

Multi-form applications are used in:

- Student management systems  
- Registration systems  
- Business software  





