# UiPath – Keyboard Automation (Simulate Keystrokes in Notepad)

This repository contains a **UiPath automation workflow** that demonstrates how to:
- **Open Notepad automatically**
- **Simulate keyboard typing (keystrokes)**
- **Use keyboard shortcuts (Ctrl + S, Alt + F4)**
- **Save and close a file** using UI Automation

---

## Project Overview
- Built using **UiPath Studio (Modern Design Experience)**
- Demonstrates use of **Start Process**, **Attach Window**, **Type Into**, and **Send Hotkey** activities
- Designed for **beginners** to understand basic **desktop keyboard automation**

---

## Workflow Logic

### Step 1 – Start Notepad
- Uses the **Start Process** activity to launch Notepad (`notepad.exe`)

### Step 2 – Type Text
- Uses **Type Into** activity with `Simulate Type` mode enabled  
- Automatically types: Yoo here bala - this is automated typing from UiPath!
- - `ClickBeforeTyping` ensures Notepad is focused before typing

### Step 3 – Save File (Ctrl + S)
- Uses **Send Hotkey** activity with:
- Key: `s`
- Modifier: `Ctrl`
- Triggers the **Save As** dialog box

### Step 4 – Enter Filename
- In the Save As dialog:
- **Type Into** the filename field:  
  `C:\Users\Public\Desktop\UiPath_AutoFile.txt`
- **Send Hotkey** → `Enter` to confirm and save

### Step 5 – Close Notepad
- Uses **Send Hotkey** activity:
- Key: `w`
- Modifier: `Alt`
- This closes Notepad automatically

---

## Example Run (Steps Overview)

| Step | Action | Description |
|------|---------|--------------|
| 1 | Launch Notepad | UiPath opens Notepad automatically |
| 2 | Type text | Simulates keystrokes to write content |
| 3 | Ctrl + S | Opens the Save As dialog |
| 4 | Type file name | Enters file name and saves file |
| 5 | Alt + F4 | Closes Notepad |

---

## Activities Used
| Activity | Purpose |
|-----------|----------|
| **Start Process** | Launches the Notepad application |
| **Attach Window** | Focuses on the Notepad or Save As window |
| **Type Into** | Types text or filename |
| **Send Hotkey** | Simulates keyboard shortcuts (Ctrl+S, Alt+F4) |
| **Delay** | Adds wait time for UI stability |

---


## OUTPUT

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/84090cff-e92e-417c-a421-8960f1d0ce43" />
<img width="1920" height="1080" alt="Screenshot 2025-11-23 124406" src="https://github.com/user-attachments/assets/7a792111-772b-4a03-8ceb-c9b30276afd6" />



---



