>>Notes-Taking-Interface-Using-C-
A console-based C++ notes app for creating, viewing, and deleting notes with text file storage. Features include ID-based organization, timestamp tracking, keyword searching, and automatic saving. Simple interface makes it easy to manage important information with minimal system requirements.

>> C++ Notes Taking Application

A simple, console-based notes taking application written in C++ that allows users to create, view, search, and delete notes with persistent storage.

>> Features

- Add Notes: Create new notes with titles and multi-line content
- View Notes: List all notes or view detailed content of a specific note
- Delete Notes: Remove unwanted notes by their ID
- Search Notes: Find notes containing specific keywords in titles or content
- Persistent Storage: All notes are automatically saved to a file and loaded when the program starts
- Timestamp Tracking: Each note is automatically timestamped when created

## Installation

>> Prerequisites
- C++ compiler (GCC, Clang, MSVC, etc.)
- Basic command line knowledge

>> Compiling the Application

1. Clone or download this repository
2. Open a terminal/command prompt and navigate to the directory containing the source code
3. Compile the application:

```bash
g++ notes_app.cpp -o notes_app
```

4. Run the application:

```bash
./notes_app    # On Linux/macOS
notes_app.exe  # On Windows
```

>> Usage Guide

The application presents a menu-driven interface:

```
===== NOTES TAKING APPLICATION =====

1. Add a new note
2. View all notes
3. View a specific note
4. Delete a note
5. Search notes
0. Exit

Enter your choice:
```

>> Adding a Note
1. Select option 1
2. Enter the title when prompted
3. Enter the content (multiple lines allowed)
4. Type "END" on a new line to finish entering content

>> Viewing Notes
- Select option 2 to see a list of all notes with their IDs, titles, and timestamps
- Select option 3 to view the complete content of a specific note (you'll need to provide the note ID)

>> Deleting Notes
1. Select option 4
2. Enter the ID of the note you wish to delete

>> Searching Notes
1. Select option 5
2. Enter a keyword to search for
3. The application will display all notes containing that keyword in either title or content

>> Exiting the Application
- Select option 0 to exit the application
- All notes are automatically saved when exiting

>> Technical Information

- Notes are stored in a file named "notes.txt" in the same directory as the executable
- Each note is assigned a unique ID automatically
- The application handles input validation to prevent crashes

>> File Format

The notes are stored in a simple text file format:
- First line: Next available ID number
- For each note:
  - ID (integer)
  - Title (text)
  - Timestamp (YYYY-MM-DD HH:MM:SS)
  - Content (can span multiple lines)
  - Separator line: "-----END_OF_NOTE-----"

>> Future Enhancements

Potential improvements for future versions:
- Note editing functionality
- Categories/tags for notes
- Rich text formatting
- Password protection
- Export to different formats (HTML, PDF, etc.)
- GUI version
