# Blogs-managment

# Blogs Management Application

## Overview

This Angular application is designed for managing programming articles in a blog format. Each article provides detailed information about a programming language, sourced from Wikipedia. The application supports article listing, adding new articles, viewing article details, adding comments, and deleting articles.

## Features

1. **Article Listing**: Displays a list of articles sorted by date (oldest first). Each article includes options to view details, add comments, or delete.
2. **Add Article**: Form to add new articles with validation and WYSIWYG text formatting options.
3. **View Detail**: Detailed view of the selected article, including comments.
4. **Add Comments**: Form to add comments to an article.
5. **Delete Article**: Confirmation pop-up for deleting an article.

## Screens

### Screen 1: Article Listing

- **Features**:
  - Displays a list of articles sorted by date.
  - Each row has buttons for:
    - **View Detail**
    - **Add Comments**
    - **Delete**
- **Date Formatting**:
  - Implemented using a custom Angular pipe to format dates as `19 Sep, 2022`.

### Screen 2: Add Article

- **Form Fields**:
  1. **Title**: Accepts only alphabetic characters.
  2. **Developed by**: Accepts only alphabetic characters.
  3. **Picture**: Upload a logo for the programming language.
  4. **Description**: Multi-line field with WYSIWYG editor for text formatting.
  5. **Rate**: Rate the article on a scale of 1-5.
  6. **Article Date**: Input date in `dd/mm/yyyy` format; formatted using a custom pipe.
- **Validation**:
  - Fields are required.
  - Validates date to ensure it is between the 21st century and the current date.
  - Displays meaningful error messages and prevents navigation away from the invalid field.

### Screen 3: View Detail

- **Features**:
  - Displays full article details and comments.
  - **Back** button redirects to the article listing view.

### Screen 4: Add Comments

- **Form Fields**:
  1. **Comment Box**: Required field for user comments.
  2. **Name**: Required field for the name of the person commenting.
- **Buttons**:
  - **Cancel**: Returns to the article listing screen.
  - **Save**: Adds the comment and returns to the article listing screen.

### Screen 5: Delete Article

- **Confirmation Pop-up**:
  - Message: "Are you sure you want to delete [Article Title]?"
  - **Ok**: Deletes the article and returns to the listing view.
  - **Cancel**: Returns to the listing view without deleting.

## Installation

To set up the project locally, follow these steps:

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/yourusername/blogs-management.git
    ```

2. **Navigate to Project Directory**:
    ```bash
    cd blogs-management
    ```

3. **Install Dependencies**:
    ```bash
    npm install
    ```

4. **Run the Application**:
    ```bash
    ng serve
    ```

5. **Open in Browser**:
    Navigate to `http://localhost:4200` to view the application.

## Usage

- **Navigate between screens** using the menu.
- **Add, view, edit, and delete articles** as described above.
- **Add comments** to articles and manage them through the user interface.

## Contributing

Feel free to submit issues and pull requests. For any major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Angular framework
- WYSIWYG editor library
- Wikipedia for programming language information

