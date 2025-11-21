⭐ Reflection Logger 4.0

Encrypted Personal Journaling Application (Windows, Closed Source)
© 2025 Soroush Sharifi – All Rights Reserved

📌 Overview

Reflection Logger 4.0 is a private, encrypted journaling and reflection tool for Windows.
It is designed for personal use and is not open-source.
Your reflections are securely stored using password-based encryption.

This project is distributed as a Windows installer (.exe) for personal use or sharing.

🛡️ Key Features

✔ Password-based encryption (Fernet)
✔ Create, edit, and view reflections
✔ Image attachments + built-in slideshow viewer
✔ Tags, search, and filtering
✔ Pinned reflections for quick access
✔ Rich-text formatting (bold, italic, underline)
✔ Emoji insertion
✔ Spell-checking
✔ Dark Mode
✔ Auto-lock on inactivity (configurable)
✔ Word & character counter
✔ Export all reflections to PDF
✔ Daily reminder if no reflection is written
✔ Backup & Restore database
✔ Windows installer support (Inno Setup)

📦 Installation

Download the latest installer from the Releases section.

Run the installer (ReflectionLoggerSetup.exe).

Follow the on-screen instructions.

Launch Reflection Logger 4.0 from your Start Menu or Desktop.

The app will automatically select the correct installation path for your system.

When you open the app for the first time after installation, it will ask for a password, which you can later change once you open the app. The password is: peasypassword

🔐 Security

Reflections are encrypted using a key derived from your password.

Password verification is based on SHA-256 hashing.

Images are stored locally and linked to encrypted entries.

Auto-lock protects your data during inactivity.

🖼️ Attachments

You can attach images to any reflection.
The app automatically:

Corrects iPhone EXIF rotation

Shrinks extremely large images

Displays thumbnails + a slideshow viewer

Shows a 📷 icon in the list for reflections with attachments

⚙️ Preferences

Accessible under Settings → Preferences

Base font size

Auto-lock timeout (0 = disabled)

Settings persist across app launches.

📂 Database

All user data is stored in:

reflection_logger.db


Attachments are stored in a subfolder next to the DB.

You may create backups or restore from an existing database using the app’s built-in tools.

💻 System Requirements

Windows 10 or Windows 11

ARM64 or x64 CPU

No additional installations required (PyInstaller bundle included)

📣 License

This is NOT an open-source project.
All rights reserved.

Copyright © 2025 Soroush Sharifi
You may not copy, modify, redistribute, or use this code or application commercially without explicit permission.

🤝 Contact

For personal inquiries or issues, please contact the author directly.
