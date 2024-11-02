# Drag and Drop Automation with Selenium

This project automates a drag-and-drop action on the jQuery UI Droppable demo page using Python, Selenium, and pytest.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Running Tests](#running-tests)
- [Code Overview](#code-overview)

## Prerequisites

- Python 3.x
- pip (Python package installer)
- A browser (Firefox, Chrome, etc.)
- WebDriver for the browser (GeckoDriver for Firefox or ChromeDriver for Chrome)

## Installation

1. Clone this repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   
## Project Structure

project_root/
│

├── drag_drop_actions.py         
Contains the Droppable class for handling the drag-and-drop functionality

└── tests/

   ├── test_drag_drop_actions.py 

Contains test cases for drag-and-drop actions

## Usage
* Open drag_drop_actions.py to understand the implementation of the Droppable class, which handles the Selenium WebDriver initialization, URL navigation, iframe handling, and drag-and-drop actions.

* Open test_drag_drop_actions.py to review the pytest test cases that validate the functionality of the Droppable class.

## Running Tests
* To execute the tests, navigate to the project root directory and run:

    ```bash
        pytest -v tests/test_drag_drop_actions.py

## Code Overview

**drag_drop_actions.py**

This file contains the Droppable class, which includes:

* get_url(): Maximizes the browser window and opens the specified URL.
* iframe(): Switches to the iframe containing the drag-and-drop elements.
* drag_drop(): Performs the drag-and-drop action from a source element to a target element.

**test_drag_drop_actions.py**

This file contains the test cases for the drag-and-drop functionality:

* test_get_url(): Asserts that the URL is opened successfully.
* test_iframe(): Asserts that the iframe is accessed successfully.
* test_drag_drop(): Asserts that the drag-and-drop action is performed without errors.