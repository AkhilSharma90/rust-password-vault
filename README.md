# Password vault with Rust


## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Dependencies](#dependencies)
4. [Usage](#usage)
    - [Menu Options](#menu-options)
5. [Code Overview](#code-overview)
    - [Main Loop](#main-loop)
    - [Add Entry](#add-entry)
    - [List Entries](#list-entries)
    - [Search](#search)
6. [File Structure](#file-structure)
7. [How to Build and Run](#how-to-build-and-run)
8. [Contributing](#contributing)
9. [License](#license)

---

## 1. Introduction <a name="introduction"></a>

Rust Password Vault is a command-line password management tool written in Rust. It allows users to securely store and manage their passwords for various services. The manager uses JSON files to store password entries.

## 2. Features <a name="features"></a>

- Add new password entries with service name, username, and password.
- List all stored entries.
- Search for entries based on service name.
- Securely stores passwords in a JSON file.

## 3. Dependencies <a name="dependencies"></a>

The project relies on Rust and Cargo for dependency management. Make sure you have Rust and Cargo installed on your system.

## 4. Usage <a name="usage"></a>

To run the program, execute the compiled binary. It will display a menu with options to perform various tasks.

### Menu Options <a name="menu-options"></a>

1. **Add Entry**: Allows the user to add a new password entry by providing the service name, username, and password.
2. **List Entries**: Displays a list of all stored password entries.
3. **Search**: Allows the user to search for entries based on the service name.
4. **Quit**: Exits the program.

## 5. Code Overview <a name="code-overview"></a>

### Main Loop <a name="main-loop"></a>

The main loop presents the menu to the user and handles their input. It dispatches the user's choice to the corresponding functionality.

### Add Entry <a name="add-entry"></a>

When the user selects to add a new entry, they are prompted for the service name, username, and password. The entry is then stored in the JSON file.

### List Entries <a name="list-entries"></a>

This option reads all entries from the JSON file and displays them in a formatted manner, including the service name, username, and password.

### Search <a name="search"></a>

The search option allows the user to input a service name to search for. It then checks all stored entries and displays any that match the search term.

## 6. File Structure <a name="file-structure"></a>

- `main.rs`: Contains the main program logic and the main loop.
- `pentry.rs`: Defines the `ServiceInfo` struct and its methods for handling password entries.

## 7. How to Build and Run <a name="how-to-build-and-run"></a>

To build and run the project, follow these steps:

1. Clone the project from [https://github.com/akhilsharma90/rust-password-vault.git](https://github.com/akhilsharma90/rust-password-vault.git).
2. Navigate to the project directory in the terminal.
3. Run `cargo build --release` to compile the project.
4. Run `./target/release/rusty_vault` to execute the compiled binary.

## 8. Contributing <a name="contributing"></a>

If you would like to contribute to this project, feel free to submit pull requests or open issues on the project's repository.

## 9. License <a name="license"></a>

This project is licensed under the [MIT License](LICENSE).
