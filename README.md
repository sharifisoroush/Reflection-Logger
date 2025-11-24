⭐ Reflection Logger 5.0

(password: peasypassword and if that doesn't work then: easypassword)

Encrypted Personal Journaling Application (Windows, Closed Source)
© 2025 Soroush Sharifi – All Rights Reserved

📌 Overview

Reflection Logger 5.0 is a private, password-protected, encrypted journaling and reflection tool for Windows.
It is designed for personal use and is not open-source.
Your reflections are securely stored using strong password-based encryption.

This project is distributed as a Windows installer (.exe) for personal use or sharing with trusted people.

🛡️ Key Features

✔ Password-based encryption using Fernet (AES + HMAC)
✔ Encrypted image attachments (full encryption, not just metadata)
✔ Create, edit, and view reflections
✔ Tags, search, and filtering
✔ Pinned reflections for quick access
✔ Rich-text formatting (bold, italic, underline)
✔ Emoji insertion
✔ Spell-checking
✔ Dark Mode
✔ Auto-lock on inactivity (configurable)
✔ Word & character counter
✔ Export all reflections to PDF
✔ Daily “write a reflection” reminder
✔ Backup & Restore database
✔ Windows installer support (Inno Setup)

🔐 Security (Updated)

Reflection Logger protects your data using multiple layers of security:

🔒 Text Encryption

Reflections are encrypted using Fernet (AES-128 in CBC mode with HMAC SHA-256).

A secure key is derived from your password using PBKDF2-HMAC-SHA256 (200,000 iterations).

Your password itself is never stored; only a SHA-256 hash is saved for verification.

🖼️ Image Encryption (NEW)

Attached images are now fully encrypted, not stored as plain files.

For each attached image:

The image is loaded from disk

iPhone EXIF rotation is automatically corrected

The image is resized (max 1024px) to reduce storage size

It is converted internally to PNG

The PNG bytes are then encrypted using the same Fernet key

The encrypted blob is stored directly inside your SQLite database

No unencrypted copies are saved.

When viewing attachments, the app decrypts and renders them on demand.

🔐 Auto-Lock

If no keyboard or mouse activity is detected, the app automatically locks based on your chosen timeout.

🖼️ Attachments

You can attach images to any reflection.

Reflection Logger automatically:

Fixes iPhone / smartphone EXIF rotation

Shrinks large images to a reasonable size

Fully encrypts them before storage

Shows thumbnails inside the preview pane

Displays a 📷 icon in the list for reflections with attachments

Provides a slideshow / image viewer via the magnifier icon

Attachments remain tied to their encrypted reflection entry.

📦 Installation

Download the latest installer from the Releases section on GitHub.

Run the installer (ReflectionLoggerSetup.exe).

Follow the on-screen instructions.

Launch Reflection Logger from your Start Menu or optional Desktop icon.

On first launch, the app will ask for a password.
You may change this password later from within the app.

Default password: peasypassword

⚙️ Preferences

Available under Settings → Preferences:

Base font size

Auto-lock timeout (0 = disabled)

Dark Mode

Spell-check toggle

All settings persist across restarts.

📂 Database

All journal data is stored in:

reflection_logger.db


Attachments are stored as encrypted blobs inside the database.
(Older versions used a folder; this version encrypts inside the DB.)

You can create backups or restore a previous database using the app’s built-in tools.

💻 System Requirements

Windows 10 or Windows 11

ARM64 or x64 CPU

No Python or dependencies required (PyInstaller bundle)
