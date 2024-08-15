# Password Manager

A simple password manager built using Python and Tkinter. This application allows users to generate secure passwords, save login credentials, and search for stored passwords.

## Features

- **Generate Password**: Creates a random, secure password with a mix of letters, numbers, and symbols.
- **Save Password**: Stores the website, email, and password in a JSON file.
- **Search Password**: Retrieves saved credentials by searching for a specific website.

## Installation

### Prerequisites

Make sure you have Python installed. This project also requires the `pyperclip` library for clipboard functionality. You can install it using pip:

```sh
pip install pyperclip
```
## Setup
- **Clone the Repository:**
  ```sh
  git clone https://github.com/AyushKanyal-me/Password-Manager.git
  cd password-manager
  ```

- **Add the Logo File:**
  Ensure you have the logo.png file in the project directory. This file is used in the UI.

- **Run the Application:**
  ```sh
    python main.py
  ```
  

## Usage

1. **Generate a Password**:
   - Click the "Generate Password" button to create a new password. The password will be copied to your clipboard and displayed in the entry field.

2. **Save a Password**:
   - Enter the website name, email/username, and generated password.
   - Click the "Add" button to save the credentials. A confirmation dialog will appear before saving.

3. **Search for a Password**:
   - Enter the website name in the search field and click the "Search" button. If the details are found, they will be displayed in a dialog box.



## Code Overview

- **Password Generation**:
  - **Function**: `generate_password`
  - **Description**: Creates a password with a random mix of letters, numbers, and symbols.
  - **Details**: Generates passwords by selecting random numbers of letters, symbols, and numbers, then shuffles them to create a secure password.

- **Save Functionality**:
  - **Function**: `save`
  - **Description**: Saves the entered website, email/username, and password into a JSON file.
  - **Details**: 
    - Checks if any fields are empty and shows an error message if so.
    - Displays a confirmation dialog before saving.
    - Updates or creates the `data.json` file with the new credentials.

- **Search Functionality**:
  - **Function**: `search_password`
  - **Description**: Retrieves and displays saved credentials based on the website name.
  - **Details**: 
    - Searches for the specified website in the `data.json` file.
    - Shows the stored email and password in a dialog box if found.
    - Displays an error message if no details are found.

- **UI Setup**:
  - **Description**: Uses the Tkinter library to create a graphical user interface.
  - **Details**:
    - **Canvas**: Displays a logo image.
    - **Labels**: Provides text fields for website, email/username, and password.
    - **Entries**: Input fields for user data.
    - **Buttons**: For generating passwords, saving credentials, and searching for passwords.


## Contributing 
Feel free to fork this repository and submit pull requests. Please make sure to follow standard coding practices and provide a clear description of your changes.

## Acknowledgements
- Tkinter for the GUI framework.
- Pyperclip for clipboard functionality.


  
