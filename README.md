# 🏥 A Command-Line Hospital Information and Patient Management System

## 📌 Project Description

**A Command-Line Hospital Information and Patient Management System** is a Python-based command-line application designed to provide basic hospital information and patient management functionalities through a simple interactive menu.

The program starts with a hospital portal and provides the user with five options: viewing admitted patients, checking assigned doctors and their departments, viewing patient consultation status, allotting a new patient, and exiting the portal.

The project demonstrates how basic Python programming concepts can be applied to a real-world hospital-management scenario.

---

## 🎯 Aim of the Project

The aim of this project is to create a simple command-line hospital portal that allows users to access basic information about patients, doctors, consultations, and new patient admissions.

The project focuses on implementing Python fundamentals in a practical application.

---

## ✨ Main Features

The program provides the following options:

### 1. 👤 Admitted Patients

The user can view a list of admitted patients and select a patient to see their details.

The available information includes:

* Patient name
* Patient ID
* Age
* Gender
* Room number
* Diagnosis
* Assigned doctor
* Contact details

The program contains four sample admitted patients.

---

### 2. 👨‍⚕️ Doctor / Department Information

The second option displays doctors assigned to different departments.

The user can select a doctor and view information such as:

* Doctor name
* Doctor ID
* Age
* Gender
* Room number
* Qualifications
* Assigned department
* Specialization
* Contact details

The program includes four doctors associated with departments such as Orthopaedics, Hepatology, Cardiology, and Gastroenterology.

---

### 3. 🩺 Consultation Status

The third option allows the user to select a patient and check their consultation status.

Depending on the selected patient, the program displays information such as:

* Consultation status
* Consultation time
* Medicines purchased

For example, the program contains both completed and pending consultation cases.

---

### 4. 🏥 New Patient Allotment

The fourth option allows the user to enter information for a new patient.

The program asks for:

* Patient name
* Patient age
* Diagnosis
* Assigned doctor

After receiving the information, the program displays a confirmation message stating that the patient has been admitted successfully.

---

### 5. 🚪 Exit

The fifth option allows the user to exit the hospital portal.

The program displays:

```text
Portal Exit Successful!!
Thank You
```

and terminates the program.

---

# 🛠️ Technologies Used

| Technology             | Purpose                                                        |
| ---------------------- | -------------------------------------------------------------- |
| Python                 | Development of the application                                 |
| Command Line Interface | Interaction with the user                                      |
| Lists                  | Storing patient and doctor information                         |
| Loops                  | Repeatedly displaying and processing menu options              |
| Conditional Statements | Handling different user choices                                |
| Input / Output         | Taking information from and displaying information to the user |
| f-strings              | Displaying formatted patient information                       |

---

# 🧠 Python Concepts Used

## 1. Variables

Variables are used to store user inputs and program data.

Examples include:

```python
a = int(input("what u wish to do today? "))
```

and:

```python
k = int(input("Enter Patient Age: "))
```

---

## 2. Lists

Lists are used to store multiple patient and doctor entries.

For example:

```python
b = ['1. Manish', '2. Rishabh', '3. Geeta', '4. Lokesh']
```

The program then displays these entries using a loop.

A similar list is used for doctors:

```python
d = ['1. Dr. Goswami', '2. Dr. Rao', '3. Dr. Singh', '4. Dr. Saxena']
```

---

## 3. Conditional Statements

The program uses `if`, `elif`, and `else` statements to determine which operation should be performed.

For example:

```python
if a == 1:
```

is used for the admitted-patient section, while:

```python
elif a == 2:
```

is used for doctor information.

Similar conditions are used for consultation status and new patient allotment.

---

## 4. While Loop

The main program uses:

```python
while 2>1:
```

to keep the hospital portal running and allow the user to select different operations.

The loop continues until the user selects the exit option.

---

## 5. For Loop

`for` loops are used to display the contents of lists.

For example:

```python
for i in b:
    print(i)
```

is used to display the admitted patients.

The doctor list and consultation-patient list are also displayed using loops.

---

## 6. User Input

The program uses the `input()` function to interact with the user.

For example:

```python
c = int(input("Select Patient: "))
```

allows the user to select a patient.

The new patient section also collects information directly from the user.

---

# 🔄 How the System Works

The basic working process of the application is:

```text
START
   ↓
Display Hospital Portal
   ↓
Display Main Menu
   ↓
Take User Choice
   ↓
 ┌───────────────────────────────┐
 │                               │
 ↓                               ↓
Choice 1                     Choice 2
Patients                     Doctors
 │                               │
 ↓                               ↓
Display Details              Display Details
 │                               │
 └───────────────┬───────────────┘
                 ↓
            Choice 3
                 ↓
       Consultation Status
                 │
                 ↓
            Choice 4
                 ↓
        New Patient Allotment
                 │
                 ↓
            Choice 5
                 ↓
                EXIT
```

---

# 📋 Main Menu

When the program starts, it displays:

```text
welcome to Sreeam hospital portal
1. Admitted Patients
2. Doctor(department) assigned
3. Consultation status
4. New Patient Allotment
5. To Exit
```

The user then enters the number corresponding to the required operation.

---

# 💻 Sample Program Execution

## Example 1 — Viewing an Admitted Patient

```text
welcome to Sreeam hospital portal

1. Admitted Patients
2. Doctor(department) assigned
3. Consultation status
4. New Patient Allotment
5. To Exit

what u wish to do today? 1

Admitted Patients:
1. Manish
2. Rishabh
3. Geeta
4. Lokesh

Select Patient: 1

Selected Patient : 1. Manish
Patient ID : P001
Age : 20
Gender : Male
Room no : AB101
Diagnosed with : Bone Fracture
Assigned Doctor : Dr. Goswami
```

---

# 👨‍⚕️ Example 2 — Viewing Doctor Information

```text
Doctors(departments) Assigned:

1. Dr. Goswami
2. Dr. Rao
3. Dr. Singh
4. Dr. Saxena

Select Doctor: 1

Selected Doctor : 1. Dr. Goswami
Doctor ID : D001
Age : 40
Gender : Male
Room no : CD101
Qualifications : MBBS, MD
Assigned Department : Orthopaedics
Specialisation in: Orthopaedic surgery
```

The corresponding doctor details are defined directly in the program.

---

# 🩺 Example 3 — Consultation Status

```text
Patient ID of Patients for consulation:

1. P026
2. P034
3. P027

Select Patient: 2

Selected Patient: 2. P034
Consultion Status: Pending
Consultation time: 10:40 am
Medicines purchased: Nil
```

The consultation section contains different statuses for the available patient IDs.

---

# 🏥 Example 4 — New Patient Allotment

```text
Enter Name of Patient: Ananya
Enter Patient Age: 25
Patient Diagnosed with: Fever
Doctor assigned: Dr. Singh

Patient Ananya under Doctor Dr. Singh has been admitted successfully

Patient ID and Room No will be generated shortly!!
```

The new-patient section accepts the required information and displays an admission confirmation.

---

# 🚪 Example 5 — Exit

```text
what u wish to do today? 5

Portal Exit Successful!!
Thank You
```

---

# 📊 Data Included in the Program

## Patient Records

The current program contains four sample admitted patients:

| Patient | ID   | Room  | Diagnosis      |
| ------- | ---- | ----- | -------------- |
| Manish  | P001 | AB101 | Bone Fracture  |
| Rishabh | P002 | AB102 | Liver Chirosis |
| Geeta   | P003 | AB103 | Chest Pain     |
| Lokesh  | P004 | AB104 | Stomach Pain   |

These records are represented directly in the program.

---

## Doctor Records

The current program contains four sample doctors:

| Doctor      | ID   | Department       |
| ----------- | ---- | ---------------- |
| Dr. Goswami | D001 | Orthopaedics     |
| Dr. Rao     | D002 | Hepatology       |
| Dr. Singh   | D003 | Cardiology       |
| Dr. Saxena  | D004 | Gastroenterology |

The program also stores their qualifications and specializations.

---

# 📁 Project Structure

A simple GitHub repository for this project can contain:

```text
A-Command-Line-Hospital-Information-and-Patient-Management-System/
│
├── anushree.py
├── README.md
└── screenshots/
    ├── main-menu.png
    ├── patient-details.png
    ├── doctor-details.png
    ├── consultation-status.png
    └── new-patient.png
```

---

# 📸 Screenshots

Screenshots of the actual program execution can be included here.

### 🏠 Main Menu

```markdown
![Main Menu](screenshots/main-menu.png)
```

### 👤 Patient Details

```markdown
![Patient Details](screenshots/patient-details.png)
```

### 👨‍⚕️ Doctor Details

```markdown
![Doctor Details](screenshots/doctor-details.png)
```

### 🩺 Consultation Status

```markdown
![Consultation Status](screenshots/consultation-status.png)
```

### 🏥 New Patient Allotment

```markdown
![New Patient](screenshots/new-patient.png)
```

---

# ⚠️ Current Limitations

The current version is a basic command-line project. Based on the provided code, patient and doctor information is predefined in the program rather than being stored in an external database or file.

Other limitations include:

* No graphical user interface
* No database connectivity
* No login/authentication system
* Patient records are predefined
* Doctor records are predefined
* No permanent data storage
* Limited input validation
* No separate admin and user roles

These limitations provide opportunities for future development.

---

# 🚀 Future Scope

The project can be enhanced in future versions by adding:

### 🗄️ Database Integration

Patient, doctor, and appointment records could be stored in SQLite or MySQL.

### 🔐 Login System

An authentication system could be added for administrators and hospital staff.

### 🖥️ Graphical User Interface

The command-line interface could be converted into a GUI using technologies such as Tkinter.

### 📅 Appointment Management

A dedicated appointment module could be developed for scheduling and managing appointments.

### 💊 Pharmacy Management

Medicine availability and patient prescriptions could be incorporated.

### 🛏️ Room Management

The system could track available and occupied hospital rooms.

### 📊 Reports

The system could generate patient and hospital reports.

---

# 🎓 Learning Outcomes

This project helped demonstrate practical use of:

* Python variables
* Lists
* Conditional statements
* `if-elif-else`
* `while` loops
* `for` loops
* User input
* Formatted output
* Basic problem-solving
* Menu-driven programming
* Real-world application design

---

# 🎯 Project Objective

The project demonstrates how a simple Python program can be designed around a real-world problem.

Instead of displaying isolated Python examples, the concepts are combined into a single application where users can interact with hospital-related information through a menu-driven system.

---

# 📝 Conclusion

The **A Command-Line Hospital Information and Patient Management System** is a basic Python application that demonstrates the implementation of fundamental programming concepts in a practical hospital scenario.

The application provides options for viewing admitted patients, checking doctor and department information, viewing consultation status, entering new patient information, and exiting the portal.

Although the current version is intentionally simple, it provides a foundation that can later be extended with databases, authentication, graphical interfaces, appointment scheduling, pharmacy management, and other advanced hospital-management features.

---

# 👨‍💻 Project Details

**Project Name:** A Command-Line Hospital Information and Patient Management System

**Programming Language:** Python

**Application Type:** Command-Line Application

**Domain:** Hospital Information and Patient Management

**Interface:** Command Line

**Purpose:** Academic / Educational Project

---

# ⭐ Acknowledgement

This project was developed as part of an academic programming project to demonstrate the practical application of Python programming fundamentals and problem-solving concepts.

---

## ⭐ Thank You

Thank you for visiting this project repository!




