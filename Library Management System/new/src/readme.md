# Library Management System

## Overview
This project is a simple **Library Management System** implemented in Java. It allows users to manage a collection of books by adding, displaying, issuing, and returning books.

## Project Structure

.vscode/
    settings.json
new/
    .vscode/
        settings.json
    bin/
    lib/
    src/
        App.java
```

### Key Files
- **[App.java]()**: Contains the main application logic for the Library Management System.
- **.vscode/settings.json**: Configuration files for the Visual Studio Code workspace.

## Features
1. **Add Book**: Add a new book to the library by providing its title and author.
2. **Display Books**: View all books in the library, including their title, author, and issued status.
3. **Issue Book**: Mark a book as issued by providing its title.
4. **Return Book**: Mark a book as returned by providing its title.
5. **Exit**: Exit the application.

## Classes

### `Book`
Represents a book in the library.

#### Attributes:
- `title`: The title of the book.
- `author`: The author of the book.
- `isIssued`: Indicates whether the book is issued.

#### Methods:
- `getTitle()`: Returns the title of the book.
- `getAuthor()`: Returns the author of the book.
- `isIssued()`: Returns the issued status of the book.
- `issueBook()`: Marks the book as issued.
- `returnBook()`: Marks the book as returned.
- `toString()`: Returns a string representation of the book.

### `Library`
Manages a collection of books.

#### Methods:
- `addBook(String title, String author)`: Adds a new book to the library.
- `displayBooks()`: Displays all books in the library.
- `issueBook(String title)`: Issues a book by its title.
- `returnBook(String title)`: Returns a book by its title.

### `App`
The entry point of the application.

#### Methods:
- `main(String[] args)`: Contains the main menu and handles user input.

## How to Run
1. Ensure you have Java installed on your system.
2. Compile the project:
   ```sh
   javac -d bin -sourcepath src src/App.java
   ```
3. Run the application:
   ```sh
   java -cp bin App
   ```

## Configuration
The project uses the following settings in `.vscode/settings.json`:
- `java.project.sourcePaths`: Specifies the source directory (`src`).
- `java.project.outputPath`: Specifies the output directory (`bin`).
- `java.project.referencedLibraries`: Includes external libraries from the `lib` folder.

## Example Usage
Library Management System
1. Add Book
2. Display Books
3. Issue Book
4. Return Book
5. Exit
Enter your choice: 1
Enter book title: The Great Gatsby
Enter book author: F. Scott Fitzgerald
Book added successfully.

## License
This project is open-source and available for educational purposes.