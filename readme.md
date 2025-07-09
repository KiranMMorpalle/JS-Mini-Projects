# 💻 JavaScript Web Projects Showcase

A collection of interactive and beginner-friendly **JavaScript projects** built with **HTML**, **CSS**, and **vanilla JS**. These projects helped me understand key concepts like DOM, events, timers, local storage, and more.

---

## 🏷️ Tech Stack

![HTML](https://img.shields.io/badge/-HTML5-orange?logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/-CSS3-blue?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/-JavaScript-yellow?logo=javascript&logoColor=black)

---

## 🔥 Projects Gallery

| Screenshot | Project | Description | Tags | Live | Code |
|-----------|---------|-------------|------|------|------|
| <img src="./ToDoApp/screenshot.png" width="120" /> | 📝 To-Do List | Add, edit, delete, and persist tasks | 🟢 Beginner · 🧠 DOM · 💾 localStorage | [Live](https://your-link.com/todo) | [Code](./ToDoApp) |
| <img src="./ColorPicker/screenshot.png" width="120" /> | 🎨 Color Picker | Pick and copy random HEX colors | 🟢 Beginner · 🧠 DOM · 🎨 UI | [Live](https://your-link.com/colorpicker) | [Code](./ColorPicker) |
| <img src="./CounterApp/screenshot.png" width="120" /> | ➕ Counter App | Increment, decrement, reset count | 🟢 Beginner · 🧠 DOM | [Live](https://your-link.com/counter) | [Code](./CounterApp) |
| <img src="./DebounceSearch/screenshot.png" width="120" /> | 🔍 Debounce Search | Search input with debounce delay | 🟡 Intermediate · 🔄 Debounce · 🔧 Events | [Live](https://your-link.com/debouncesearch) | [Code](./DebounceSearch) |
| <img src="./Calculator/screenshot.png" width="120" /> | 🧮 Calculator | Basic math operations with logic | 🟡 Intermediate · 🧠 DOM | [Live](https://your-link.com/calculator) | [Code](./Calculator) |
| <img src="./FormValidation/screenshot.png" width="120" /> | 📧 Form Validator | Validates email/password inputs | 🟢 Beginner · 🧠 Regex · 🧾 Forms | [Live](https://your-link.com/formvalidation) | [Code](./FormValidation) |

> ℹ️ Add your screenshots as `screenshot.png` inside each project folder for auto-display.

---

## 📁 Folder Structure
```
📦 JS-Web-Projects
├── ToDoApp/
│ └── screenshot.png
├── ColorPicker/
│ └── screenshot.png
├── CounterApp/
│ └── screenshot.png
```

---

## 🔄 Auto-Update Table Script (Optional)

Want to generate the project table dynamically? Here's a Python script:

```python
import os

def get_projects_table():
    rows = []
    base_url = "https://your-link.com"

    for project in os.listdir('.'):
        if os.path.isdir(project) and project not in ['.git', '.github']:
            name = project.replace('-', ' ').title()
            screenshot_path = f"{project}/screenshot.png"
            if os.path.exists(screenshot_path):
                screenshot = f'<img src="./{screenshot_path}" width="120" />'
            else:
                screenshot = "No preview"
            live = f"[Live]({base_url}/{project.lower()})"
            code = f"[Code](./{project})"
            desc = "Your description here"
            tags = "🟢 Beginner · 🧠 DOM"
            rows.append(f"| {screenshot} | {name} | {desc} | {tags} | {live} | {code} |")

    return "\n".join(rows)

print(get_projects_table())

---

Let me know if you'd like me to:
- Add a **Notion template tracker**
- Set up a **GitHub Action to auto-run the script**
- Create a **blog integration section**

Would you like me to generate this template as a ready-to-clone repo with starter folders, screenshot placeholders, and the Python script included?

