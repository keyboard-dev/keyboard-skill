# Keyboard Skill for Claude

This repository contains documentation designed to be imported into **Claude.ai** as a custom "skill" or persistent knowledge base using the **Projects** feature.

---

## 🚀 How to Import into Claude

To give Claude these keyboard capabilities, follow these steps:

### 1. Prepare the File
Ensure you have the `keyboard.md` file downloaded from this repository to your local machine.

### 2. Create a Project in Claude
* Log into [Claude.ai](https://claude.ai).
* On the left sidebar, click on **Projects**.
* Select **"Create Project"** and name it (e.g., *Keyboard Specialist*).

### 3. Upload the Knowledge
* Inside your new project, click the **"Add Content"** button (or drag and drop).
* Upload the `keyboard.md` file. 
* Claude will now process this file as part of its "Project Knowledge."

### 4. Set Custom Instructions (Recommended)
In the **"Project Instructions"** text box on the right, add the following to ensure Claude uses the file correctly:
> *"Always reference the attached keyboard.md file when answering questions about shortcuts or navigation. If a conflict exists between your general knowledge and this file, prioritize the file."*

> **Note:** This method requires a **Claude Pro** or **Team** subscription to access the Projects feature. If you are on the Free tier, you can simply attach the Markdown file to individual chat sessions manually.
