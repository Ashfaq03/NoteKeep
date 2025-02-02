# NoteKeep

NoteKeep is a simple and intuitive note-taking web application built using HTML, CSS, and JavaScript. It allows users to create, edit, and delete notes, with data saved locally in the browser using `localStorage`.

## 🚀 Features

- **Create Notes:** Add new notes instantly with a click.
- **Edit Notes:** Notes are editable directly in the browser.
- **Delete Notes:** Remove notes easily with a delete icon.
- **Auto-Save:** Changes are automatically saved using `localStorage`.
- **Persistent Data:** Notes remain intact even after refreshing the page.

## 🛠️ Technologies Used

- **HTML:** Structure of the web app.
- **CSS:** Styling to enhance the user interface.
- **JavaScript:** Core functionality for creating, editing, deleting, and saving notes.

## 📦 How to Run Locally

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/NoteKeep.git
   ```
2. **Navigate to the Project Folder:**
   ```bash
   cd NoteKeep
   ```
3. **Open `index.html` in Your Browser:**
   - You can double-click the `index.html` file, or
   - Run it using Live Server in VS Code.

## 📋 Usage

- Click on the **"Create Note"** button to add a new note.
- Type your content directly in the note.
- Click the **delete icon** to remove a note.
- Notes are saved automatically; no need to manually save.

## 🔑 Key Code Snippets

- **Saving Notes to Local Storage:**
  ```javascript
  function updateStorage() {
    localStorage.setItem("notes", notesContainer.innerHTML);
  }
  ```
- **Creating a New Note:**
  ```javascript
  createNoteBtn.addEventListener("click", () => {
    let inputBox = document.createElement("p");
    let img = document.createElement("img");
    inputBox.className = "input-box";
    inputBox.setAttribute("contenteditable", "true");
    img.src = "./assets/delete.png";
    notesContainer.appendChild(inputBox).appendChild(img);
  });
  ```

## 📁 Folder Structure

```
NoteKeep/
├── index.html
├── style.css
├── script.js
└── assets/
    └── delete.png
```

## ✨ Future Improvements

- Add color-coding for notes.
- Implement a search functionality.
- Enable cloud synchronization.
- Add dark mode support.

## 🙌 Contributing

Contributions are welcome! Feel free to fork this repository, make changes, and submit pull requests.

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

**Developed by [Syed Ashfaquddin](https://github.com/Ashfaq03) 🚀**

