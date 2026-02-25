# 📝 Task Board App (To-Do List v2)

A more advanced **Task Board application** built with **Vanilla JavaScript**, featuring task tags, creation date tracking, dynamic rendering, and LocalStorage persistence.

This project represents an evolution of a basic To-Do List, focusing on cleaner architecture, improved UI structure, and better state handling.

---

## ✨ Features

- ✅ Create new tasks
- 🏷️ Add tags to tasks
- 📅 Automatic creation date
- ✔️ Mark tasks as completed
- 🖼️ Visual completed icon indicator
- 💾 Persistent storage using LocalStorage
- 📊 Dynamic progress counter
- 🎨 Card-style task layout
- 🔄 Automatic UI re-rendering

---

## 🛠️ Technologies Used

- HTML5
- CSS3
- JavaScript (ES6+)
- LocalStorage API

---

## 🧠 Concepts Applied

This project demonstrates:

- DOM element creation with `document.createElement`
- Dynamic rendering patterns
- State synchronization with LocalStorage
- Array methods (`map`, `filter`, `forEach`)
- ID generation logic
- Conditional rendering
- Form handling and validation
- Clean function separation
- Component-like rendering structure

---

## 📂 Project Structure

📦 to-do-list-project02  
 ┣ 📂 .vscode  
 ┃ ┗ 📜 settings.json  
 ┣ 📜 Checked.png  
 ┣ 📜 index.html  
 ┣ 📜 index.js  
 ┣ 📜 style.css  
 ┗ 📜 README.md  

---

## 🔍 How It Works

### 📦 Task Data Structure

Each task is stored as an object:

```
{
  id: number,
  name: string,
  tag: string,
  createdAt: string,
  completed: boolean
}
```

---

## 🔢 ID Generation

The application automatically generates incremental IDs:

- It reads existing tasks
- Gets the last task ID
- Adds +1 to generate the next ID

This ensures unique identifiers for each task.

---

## 🧱 Rendering System

Tasks are dynamically rendered using:

- `createTaskElement(task)`
- `renderTasks()`
- `renderTasksProgressData(tasks)`

The app clears and re-renders the list whenever the state updates, ensuring UI consistency.

---

## 🏷️ Task Card Structure

Each task is rendered as a structured card containing:

- Task title
- Tag label
- Creation date
- Complete button (if pending)
- Completed icon (if finished)

---

## 📊 Progress Counter

The footer dynamically displays:

```
X completed out of Y tasks
```

It updates whenever:

- A task is created
- A task is completed
- The page reloads

---

## 💾 LocalStorage Integration

Core functions:

```
getTasksFromLocalStorage()
setTasksInLocalStorage(tasks)
```

Tasks persist even after refreshing the browser.

---

## 🧪 How to Run Locally

1. Clone the repository:

```
git clone https://github.com/Brunacardosof/to-do-list-project02.git
```

2. Navigate to the folder:

```
cd to-do-list-project02
```

3. Open `index.html` in your browser  
   or use Live Server (default port: 5501)

---

## 🎯 Project Evolution

Compared to the previous version, this project introduces:

- Better UI structure
- More scalable rendering logic
- Tag system
- Date tracking
- Improved separation of concerns
- Cleaner state management

---

## 👩‍💻 Author

Bruna Cardoso  
GitHub: https://github.com/Brunacardosof

---

## 📄 License

This project is licensed under the MIT License.
