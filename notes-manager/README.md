# 📝 Notes Manager

A lightweight, browser-based notes and documentation management tool. No server or installation required — just open `index.html` in any modern browser.

## Features

| Feature | Description |
|---|---|
| ✏️ **Create notes** | Write and save notes with a title and body |
| 📂 **Topic organisation** | Group notes under custom topics (e.g. Work, Personal, Learning) |
| 🔍 **Search** | Instantly filter notes by title, content, or topic |
| 👁 **Read view** | Click any note card to read it in a focused view |
| ✏️ **Edit** | Update any note at any time |
| 🗑 **Delete** | Remove individual notes or entire topics (notes are kept, just untagged) |
| 💾 **Persistent storage** | All notes are saved in the browser's `localStorage` — they survive page refreshes |

## How to Use

### Open the app
1. Navigate to the `notes-manager/` folder.
2. Open `index.html` in your browser (double-click the file, or use *File → Open* in your browser).

### Create a note
1. Click the **+ New Note** button in the top-right corner.
2. Fill in the **Title**, select a **Topic** (optional), and write your **Content**.
3. Click **Save Note**.

### Create a topic
1. Click inside the **New topic** input at the bottom of the left sidebar.
2. Type the topic name and press **Enter**.

### Search notes
Use the search bar in the toolbar to filter notes in real time across titles, content, and topics.

### Edit a note
- Hover over a note card and click the ✏️ icon, **or**
- Click the note card to open the full view, then click **✏️ Edit**.

### Delete a note
- Hover over a note card and click the 🗑 icon, **or**
- Open the full view and click **🗑 Delete**.

### Delete a topic
Hover over a topic in the sidebar and click the ✕ button. Notes tagged with that topic will be kept but untagged.

## Storage

All data is stored in your browser's **localStorage** under the key `notes_manager_v1`. Clearing your browser data will remove all notes. To back up your notes, copy the value from the browser console:

```js
localStorage.getItem('notes_manager_v1');
```

Paste the JSON into a file to keep a backup, and restore it with:

```js
localStorage.setItem('notes_manager_v1', '<paste JSON here>');
```

## Browser Compatibility

Works in any modern browser: Chrome, Firefox, Edge, Safari, Brave.
