# 📝 To-Do List Application

A beautiful, feature-rich to-do list application with **local storage persistence**, priority levels, and task filtering.

## ✨ Features

- ✅ **Add Tasks** - Create new tasks with a modal form
- ✅ **Edit Tasks** - Modify existing tasks and their priorities
- ✅ **Delete Tasks** - Remove individual tasks with confirmation
- ✅ **Mark Complete** - Check off completed tasks
- ✅ **Priority Levels** - Set Low, Medium, or High priority for each task
- ✅ **Filter Tasks** - View All, Active (pending), or Completed tasks
- ✅ **Statistics Dashboard** - Track total, completed, and pending tasks
- ✅ **Local Storage** - All data persists automatically in browser
- ✅ **Responsive Design** - Works perfectly on desktop, tablet, and mobile
- ✅ **Keyboard Support** - Press Enter to add tasks quickly
- ✅ **Smooth Animations** - Beautiful fade-in and slide transitions

## 🎨 Design Highlights

- **Modern UI** - Clean, gradient-based interface with purple theme
- **Color-Coded Priorities** - Visual indicators for task urgency
  - 🔴 High (red background)
  - 🟡 Medium (yellow background)
  - 🟢 Low (green background)
- **Empty States** - Helpful messaging when no tasks exist
- **Hover Effects** - Interactive feedback on all buttons and items
- **Accessibility** - Semantic HTML, proper labels, and keyboard navigation

## 🚀 Quick Start

### Option 1: Open Directly
Simply open `todo-app.html` in your web browser. No installation required!

### Option 2: View Online
Access via GitHub Pages (if deployed):
```
https://bordin13.github.io/odr-geospatial-portal/todo-app.html
```

### Option 3: Clone & Run
```bash
git clone https://github.com/bordin13/odr-geospatial-portal.git
cd odr-geospatial-portal
# Open todo-app.html in your browser
```

## 📖 How to Use

### Adding a Task
1. Type your task in the input field at the top
2. Click the **"Add"** button or press **Enter**
3. Fill in the task details and priority in the modal
4. Click **"Save Task"**

### Editing a Task
1. Click the **✏️ Edit button** on any task
2. Update the description and/or priority
3. Click **"Save Task"**

### Completing a Task
- Click the **checkbox** next to any task to mark it complete
- Completed tasks appear faded with strikethrough text

### Deleting a Task
- Click the **🗑️ Delete button** on any task
- Confirm the deletion in the dialog

### Filtering Tasks
- Click **"All"** to see all tasks
- Click **"Active"** to see only pending tasks
- Click **"Completed"** to see only finished tasks

### Statistics
- **Total** - Total number of tasks
- **Completed** - Number of finished tasks
- **Pending** - Number of active tasks

### Clear Completed
- Click **"Clear All Completed"** to remove all finished tasks at once

## 💾 Local Storage

All tasks are automatically saved to your browser's local storage:

```javascript
// Data structure
{
  id: 1234567890,
  text: "Buy groceries",
  priority: "high",
  completed: false,
  createdAt: "2026-04-28T01:16:02.000Z"
}
```

**Features:**
- ✅ Automatic saving after every action
- ✅ Data persists across browser sessions
- ✅ No internet connection required
- ✅ ~5-10MB storage per domain

**Important:**
- Clearing browser cache/cookies will delete all tasks
- Storage is per-browser (not synced across devices)
- Use browser DevTools → Application → Local Storage to view raw data

## 🎯 Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| Enter (in input) | Open Add Task modal |
| Escape (in modal) | Close modal |
| Tab | Navigate between fields |

## 🛠️ Technical Details

### Technologies Used
- **HTML5** - Semantic markup
- **CSS3** - Modern styling with gradients, animations, flexbox
- **Vanilla JavaScript** - No frameworks or dependencies
- **Local Storage API** - Browser-native persistence

### Code Structure
```javascript
// Key Functions
loadTasks()           // Load from localStorage
saveTasks()           // Save to localStorage
openAddModal()        // Show add task dialog
saveTask(e)          // Save/update task
toggleTask(id)       // Mark complete/incomplete
deleteTask(id)       // Remove task
filterTasks(filter)  // Show all/active/completed
renderTasks()        // Update UI
updateStats()        // Refresh statistics
```

### File Size
- **Total:** ~18KB (uncompressed)
- **HTML:** ~2KB
- **CSS:** ~8KB (including animations)
- **JavaScript:** ~8KB (including storage logic)

## 🎨 Customization

### Change Color Scheme
Edit the gradient in the `body` CSS:
```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

### Modify Priority Colors
Update the priority classes in CSS:
```css
.priority-high { background: #ffe0e0; color: #c92a2a; }
.priority-medium { background: #fff3bf; color: #d9a804; }
.priority-low { background: #d3f9d8; color: #2b8a3e; }
```

### Add New Features
- Add due dates: Add `dueDate` property to task object
- Add categories/tags: Extend filter logic
- Add task notes: Add description modal field
- Export/Import: Add JSON download functionality

## 📱 Browser Compatibility

| Browser | Support |
|---------|---------|
| Chrome | ✅ Full |
| Firefox | ✅ Full |
| Safari | ✅ Full |
| Edge | ✅ Full |
| Opera | ✅ Full |
| IE 11 | ⚠️ Limited |

**Requirements:**
- Local Storage API support
- CSS Grid/Flexbox support
- ES6 JavaScript support

## 🐛 Troubleshooting

### Tasks not saving?
- Check if Local Storage is enabled in browser settings
- Verify browser isn't in private/incognito mode
- Try clearing browser cache and reloading

### Tasks disappeared after restart?
- Browser cache was cleared (tasks stored in Local Storage)
- Try opening DevTools → Application → Local Storage to check
- If using private browsing, data won't persist

### Modal not opening?
- Ensure JavaScript is enabled
- Try refreshing the page
- Check browser console for errors (F12)

## 📚 Learning Resources

### Local Storage API
- [MDN Web Docs - Local Storage](https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage)
- [Web Storage Guide](https://www.w3schools.com/html/html5_webstorage.asp)

### JavaScript Concepts Used
- Array methods: `map()`, `filter()`, `find()`
- JSON: `stringify()`, `parse()`
- Event listeners: `addEventListener()`
- DOM manipulation: `querySelector()`, `classList`

## 🚀 Future Enhancements

- [ ] Task categories/tags
- [ ] Due dates and reminders
- [ ] Recurring tasks
- [ ] Task notes/descriptions
- [ ] Export to JSON/CSV
- [ ] Dark mode toggle
- [ ] Cloud sync
- [ ] Drag-to-reorder
- [ ] Search functionality
- [ ] Statistics charts

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](../LICENSE) file for details.

## 👤 Author

**bordin13** - [GitHub Profile](https://github.com/bordin13)

## 🙏 Acknowledgments

- Inspired by modern productivity apps
- Built with vanilla JavaScript for learning purposes
- Perfect for portfolio projects

---

**Happy task managing!** 📝✨
