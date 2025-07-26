# 🗂️ Batch File to Create Project Folders, Subfolders, and Files

> Automate your project setup with a simple batch script — ideal for developers working on structured PHP-based projects like **School Fee Manager**.

## 📋 Overview

When starting a new project, organizing your files and folders properly is crucial for smooth development. This repository provides a **Windows batch script** that automatically creates a complete folder and subfolder structure, along with placeholder PHP files, for a sample project called `School Fee Manager`.

## ⚙️ What Is a Batch File?

A **batch file** (`.bat`) is a script file that contains a sequence of commands to be executed by the Windows Command Prompt (`cmd.exe`). It is commonly used for automating tasks such as:

- Creating directories and files
- Running programs
- Setting environment variables

## 🎯 Why Use a Batch File for Project Setup?

Using a batch file to initialize your project structure has several benefits:

- ✅ **Saves Time**: Automates directory and file creation in seconds.
- ✅ **Reduces Human Error**: Prevents typos and missing files.
- ✅ **Standardizes Structure**: Ensures consistency across teams and projects.
- ✅ **Easy to Share**: Share one `.bat` file and replicate the structure anywhere.
- ✅ **Reusability**: Use and tweak the script for future projects.

## 🧾 Script Details

This batch file will create a directory named `school_fee_manager` with a full subfolder and PHP file structure inside.

### 🔧 Script: `create_project_structure.bat`

```bat
@echo off

cd /d "%~dp0"
mkdir school_fee_manager
cd school_fee_manager
mkdir assets
mkdir includes
mkdir attendance
mkdir students
mkdir fees

type nul > index.php

cd includes
type nul > config.php
type nul > db_connect.php
type nul > header.php
type nul > footer.php

cd ../attendance
type nul > mark_attendance.php
type nul > report.php
type nul > class_report.php

cd ../students
type nul > add.php
type nul > edit.php
type nul > view.php
type nul > view_all.php

cd ../fees
type nul > due.php
type nul > pay.php
type nul > receipt.php
type nul > payment_history.php
type nul > individual_history.php

echo folders and files has been created
pause
````

## 📂 Generated Folder Structure

```
school_fee_manager/
│
├── index.php
├── assets/
├── includes/
│   ├── config.php
│   ├── db_connect.php
│   ├── header.php
│   └── footer.php
├── attendance/
│   ├── mark_attendance.php
│   ├── report.php
│   └── class_report.php
├── students/
│   ├── add.php
│   ├── edit.php
│   ├── view.php
│   └── view_all.php
└── fees/
    ├── due.php
    ├── pay.php
    ├── receipt.php
    ├── payment_history.php
    └── individual_history.php
```

## 🚀 How to Use

1. Open **Notepad** or any text editor.
2. Paste the batch script above.
3. Save the file with a `.bat` extension (e.g., `create_project_structure.bat`).
4. Double-click the file to execute and create the folder structure.

## 🛠️ Customization

Feel free to modify folder names and files to match your own project requirements. This batch file serves as a template for setting up many types of structured web or software projects.

## 🧑‍💻 Author

**Xitiz Basnet**
Feel free to [connect with me](https://github.com/xitizbasnet) on GitHub.

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

