# ElevateLab-Task02
Built a To-Do List Web App (Front-end only, using Vanilla JavaScript)

# To-Do List Web App

A simple and functional To-Do List application built with vanilla JavaScript, HTML, and CSS. This project demonstrates core web development concepts including DOM manipulation, event handling, and dynamic UI updates.

## 📋 Project Overview

This is a front-end only To-Do List application that allows users to:
- Add new tasks
- Mark tasks as complete/incomplete
- Delete tasks
- View all tasks in a clean interface

## 🛠️ Technologies Used

- **HTML5** - Structure and layout
- **CSS3** - Styling and responsive design
- **Vanilla JavaScript** - Functionality and interactivity

## ✨ Features

- ✅ Add new tasks using button or Enter key
- ✅ Toggle task completion with checkboxes
- ✅ Delete individual tasks
- ✅ Real-time UI updates without page reload
- ✅ Clean and simple user interface
- ✅ Responsive design

## 🚀 How to Run

1. Clone this repository or download the files
2. Open `index.html` in any modern web browser
3. Start adding tasks!

No installation or setup required - just open and use!

## 📂 File Structure

```
todo-list-app/
│
├── index.html          # Main HTML file with embedded CSS and JavaScript
└── README.md           # Project documentation
```

## 💡 Key Concepts Demonstrated

### 1. DOM Manipulation
- Selecting elements using `getElementById()`
- Creating elements dynamically with `createElement()`
- Appending elements to the DOM with `appendChild()`

### 2. Event Listeners
- Button click events
- Keyboard events (Enter key)
- Event delegation for dynamically created elements

### 3. JavaScript ES6 Features
- `let` and `const` for variable declarations
- Array methods: `push()`, `filter()`, `find()`, `forEach()`
- Template literals and string methods

### 4. Event Delegation
- Single event listener on parent element handles all task interactions
- Efficient handling of dynamically added elements

### 5. State Management
- Tasks stored in JavaScript array
- UI updates based on state changes

## 🎯 Functionality Breakdown

### Adding Tasks
- User enters task text in input field
- Clicks "Add" button or presses Enter
- Task is added to tasks array
- UI updates to display new task

### Completing Tasks
- User clicks checkbox next to task
- Task's completed status toggles
- Visual indication (strikethrough text, background color change)

### Deleting Tasks
- User clicks "Delete" button on task
- Task is removed from tasks array
- UI updates to remove task from display

## 📝 Code Highlights

**Event Delegation Example:**
```javascript
taskList.addEventListener('click', function(e) {
    const taskItem = e.target.closest('.task-item');
    if (!taskItem) return;
    
    // Handle checkbox or delete button clicks
});
```

**Dynamic Task Creation:**
```javascript
const li = document.createElement('li');
li.className = 'task-item';
li.dataset.id = task.id;
// Add checkbox, text, and delete button
taskList.appendChild(li);
```
