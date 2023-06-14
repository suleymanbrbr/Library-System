# Library-System

Introduction
In this assignment, you will develop a library management program to handle a collection of books. The main functionalities include adding books to the library, searching for a book by author, searching for a book by title and displaying the books sorted by the author's last name. If multiple books have the same author, they will be sorted by their titles. You will implement the insertion sort algorithm to sort the books, the binary search algorithm to search for a book by the author, and the linear search algorithm to search by title. This project aims to provide practice working with structs and vectors. You can utilize the algorithms provided in your lectures to complete this task.

Inputs
There are various inputs in this program, including book details, menu choices, and search queries. The primary inputs are the book's title, author, and publication year. You can assume that the book's title and author will be strings containing letters, digits, and spaces. The publication year will be an integer input. The user can add books one at a time using the "Add books" menu option.
Another input is the menu choice, which is an integer ranging from 1 to 5, representing the available menu options. The user can enter menu choices until they enter "5" to quit the program.
The search query is a string input representing the title of the book the user wants to search for.
Input Checks
The rules for input checks are as follows:
For book details and search query, you can assume that the user enters these inputs correctly, and you do not have to check them.
Book details:
Title: Must be a string containing only letters, digits, and spaces. Author: Must be a string containing only letters, digits, and spaces. Publication Year: Must be a valid integer.
Search query:
Must be a string containing only letters, digits, and spaces. Cannot be empty.
You can assume that the menu choice is an integer, but you should check it for the range. Menu choice: Must be an integer ranging from 1 to 5.
In case of an invalid input, the program should ask for input again until a correct input is entered. Use loops and conditional statements to ensure input validity.
 Processing, Program Flow, and Output
Your program should start with an introductory explanation and a prompt for the input. After initializing the library system with a predefined set of books, the program will display a menu with four options:
     Library System Menu:
     1. Add books
     2. Search for an author
     3. Search for by book title
     4. Display books
5. Quit
The user can enter their choice as an integer.
And here is the predefined set of books that you should implement into your code:
     vector<Book> books = {
             {"The Great Gatsby", "F Scott Fitzgerald", 1925},
             {"Moby Dick", "Herman Melville", 1851},
             {"To Kill a Mockingbird", "Harper Lee", 1960},
             {"Pride and Prejudice", "Jane Austen", 1813},
             {"Burmese Days", "George Orwell", 1934},
             {"Brave New World", "Aldous Huxley", 1932},
             {"Animal Farm", "George Orwell", 1945}
};
If the user chooses to add a book, the program should prompt for the book's title, author, and publication year. After the user enters the details, the program should add the book to the library and re-sort the library.
If the user chooses to search for a book by an author, the program should prompt for the author's full name. The search should be based on the author's last name and be case-insensitive. If any books are found by the specified author, the program should display the details of each book, including its title, author, publication year and position. If no books are found by the specified author, the program should display an appropriate message.
If the user chooses to search for a book by title, the program should prompt for the book's title. The search should be case-insensitive and based on the provided title. If any books with the specified title are found, the program should display the details of each book, including its title,

author, publication year, and position in the sorted list. If no books are found with the specified title, the program should display an appropriate message.
If the user chooses to display books, the program should display the entire library sorted by the author's last name as case-insensitive. The output should include the book's title, author, and publication year.
If the user chooses to quit, the program should display a farewell message and terminate.
Your program should continuously display the menu and prompt for input until the user chooses to quit.
In this homework assignment, it is required to store the book data in a structured way, using a struct and a vector. This will help keep the data organized and make it easier to perform various operations on the data, such as sorting, searching, and displaying.
A struct is a composite data type that groups together variables under a single name, making it easier to manage related data. In this case, a struct called Book has been defined with three members: title, author, and publication year. Each member holds a piece of information about a book.
A vector is a dynamic array that can grow or shrink in size as elements are added or removed. In this assignment, a vector of Book structs is used to store the book data. This allows for easy management of the book collection and enables the use of various vector operations, such as adding a new book or searching for an existing one.
