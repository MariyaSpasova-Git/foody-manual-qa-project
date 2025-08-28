# Software Requirements

## Purpose and Scope
The "Foody" application is a web platform that allows users to register, log in, and manage their food-related content. The document describes core functionalities for both unregistered and registered users, but does not cover administrative features.

## System Overview
The app has two main user types:

- **Unregistered Users**: Can only access the main Home Page, which provides links to sign up or log in.
- **Registered Users**: Have access to all main functionalities, including profile management and creating/managing food entries.

The application is hosted at the URL: http://softuni-qa-loadbalancer-2137572849.eu-north-1.elb.amazonaws.com:85

## Key Features

### User Account Management
- **Registration (Sign Up)**: Users can create an account by providing a username, email, first name, last name, and a password. Specific constraints apply to each field (e.g., username must be 2-30 characters, email must be in a valid format).

- **Log In**: Registered users can sign in using their username and password. A "Forgot Password" feature is also available.

- **Profile Management**: Logged-in users can edit their profile page, which includes updating their first, middle, and last names, "About me," "About my food passion," and a profile picture via a URL. The page also displays their total food count.

### Food Content Management
- **Food Creation**: Registered users can create a new food entry by providing a title, description, and a picture URL.

- **Home Page (Logged In)**: The home page for registered users shows a welcome message and a search bar to filter foods by title. It lists all of the user's created foods. If no foods have been created, a message "There are no foods :(" is displayed.

- **Food Management**: On the home page, each created food entry has dedicated buttons for:
    - View: To view the food details.
    - Edit: To modify the food entry.
    - Delete: To remove the food entry from the app.