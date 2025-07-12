Online Library System 📚
An interactive web application built with React for the frontend, utilizing Redux for centralized state management and React Router for seamless navigation. This system allows users to browse books by categories, search for books by title or author, view detailed information about each book, and add new books via a validated form.

✨ Features
Home Page: Welcome message, a list of book categories, and a display of popular books with links to their details.

Browse Books Page:

Displays a list of books with dynamic filtering by category (e.g., /browse-books?category=Fiction).

Search functionality to filter books by title or author.

Links from each book to its detailed view.

Book Details Page: Shows comprehensive information (title, author, description, rating) for a selected book via a dynamic route. Includes a "Back to Browse" button.

Add Book Page: A form for adding new books to the library.

Utilizes Redux for state management to add new books to the global list.

Redirects to the Browse Books page upon successful submission, displaying the newly added book.

Includes client-side form validation to ensure all fields are correctly filled.

404 Page: A "Page Not Found" route for undefined URLs, with a link back to the Home page.

🚀 Technologies Used
React: Frontend JavaScript library for building user interfaces.

Redux: Predictable state container for managing application state.

React Router: Declarative routing for React.

UUID: For generating unique IDs for new books.

CSS: For styling the application.

📦 Setup and Installation
Follow these steps to get the project up and running on your local machine.

Clone the repository:

git clone https://github.com/Pankaj-Baraiya/online-library-system.git

(Replace Pankaj-Baraiya with your actual GitHub username if different).

Navigate to the project directory:

cd online-library-system

Install dependencies:
This command installs all the necessary packages (React, Redux, React Router, UUID) listed in package.json.

npm install

▶️ How to Run the Application
Once the dependencies are installed, you can start the development server:

npm start

This command will:

Start the development server.

Open your default web browser.

Load the application at http://localhost:3000 (or another available port if 3000 is in use).

The application will automatically reload if you make any changes to the source code.

📂 Project Structure
online-library-system/
├── public/
├── src/
│   ├── actions/
│   │   └── bookActions.js     # Redux actions for books
│   ├── components/
│   │   ├── BookCard.js        # Reusable component for displaying a single book
│   │   ├── NavigationBar.js   # Main navigation bar
│   │   ├── BookCard.css
│   │   └── NavigationBar.css
│   ├── pages/
│   │   ├── AddBookPage.js     # Form to add new books
│   │   ├── BookDetailsPage.js # Displays detailed info of a single book
│   │   ├── BrowseBooksPage.js # Lists books with search/filter
│   │   ├── HomePage.js        # Landing page with categories and popular books
│   │   ├── NotFoundPage.js    # 404 error page
│   │   ├── AddBookPage.css
│   │   ├── BookDetailsPage.css
│   │   ├── BrowseBooksPage.css
│   │   ├── HomePage.css
│   │   └── NotFoundPage.css
│   ├── reducers/
│   │   └── bookReducer.js     # Redux reducer for book state
│   ├── store.js               # Redux store configuration
│   ├── App.js                 # Main application component, handles routing
│   ├── App.css                # Global CSS for the app
│   └── index.js               # Entry point of the React application
├── package.json               # Project dependencies and scripts
└── README.md                  # This file

🤝 Contributing
Contributions are welcome! If you have suggestions or want to improve the project, feel free to fork the repository and submit a pull request.

📄 License
This project is open source and available under the MIT License.
