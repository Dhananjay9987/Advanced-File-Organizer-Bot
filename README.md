# Project Title:

Advanced File Organizer Bot

# Problem Statement:

Modern users often deal with cluttered download folders or directories full of random
files. Manually organizing them by file type, size, or extension is time-consuming. This
project addresses this problem by providing a real-time automated file organizer that
monitors a folder and instantly sorts new files as they arrive.

# Project Overview:

This Python-based desktop application allows users to select a folder and automatically
Organize files based on:
  • File extension (e.g., .jpg, .pdf)
  • File type (e.g., image, document, video)
  • File size (small, medium, large)
It also provides real-time monitoring using the Watchdog library, meaning new files are
sorted instantly as they are added. The tool comes with a Tkinter-based GUI, allowing
users to start organizing without typing a single command.

# Key Features:

Feature        ----------      Description

1. Folder Selection ----------  User selects any folder via a GUI
2. Sort by Extension ---------- Sorts files into folders like JPG_Files, PDF_Files, etc.
3. Sort by File Type ---------- Categorizes files as Image, Video, Document, or Other
4. Sort by File Size ---------- Categorizes files as Small, Medium, or Large
5. Real-Time Monitoring ------- Uses Watchdog to monitor a folder and organize new files as they appear
6. GUI Interface (Tkinter) ---- Easy-to-use interface with checkboxes and buttons

# Technologies Used:

1. Python 3:- Core logic and programming language
2. Tkinter:- Building the graphical user interface (GUI)
3. Watchdog:- Real-time monitoring of file system changes
4. shutil, os:- File operations like moving and creating directories
5. filedialog:- GUI dialog for folder selection

# Core Logic:

• Organizing Strategy:
  o By extension: Groups files like pdf, jpg, etc.
  o By type: Uses predefined extensions to classify into Image, Video, Document.
  o By size: Groups as Small (<1MB), Medium (1–10MB), Large (>10MB)
• Live Monitoring:
  o Uses Observer and FileSystemEventHandler from watchdog to listen for new files.
  o When a new file is created, it is instantly categorized based on selected options.
• GUI Flow:
  o Users choose folder → select sorting preferences → click "Start Monitoring"
  o Once active, the tool silently organizes incoming files.

# What You Learned:

• Building GUI applications with checkboxes, buttons, and dialogs using Tkinter
• Implementing event-driven file system monitoring using Watchdog
• Performing file operations (move, rename, create folders) using os and shutil
• Structuring Python applications with clear logic separation
• Handling file type inference, extension parsing, and robust exception handling
• Delivering a real-world productivity automation tool
