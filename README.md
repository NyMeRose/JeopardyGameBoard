# JeopardyGameBoard

This project is a simple Jeopardy game built using HTML, CSS, and JavaScript.  It uses jQuery for DOM manipulation and AJAX requests.

## Table of Contents

-   [Demo](#demo)
-   [Features](#features)
-   [Installation](#installation)
-   [Usage](#usage)
-   [Data Source](#data-source)
-   [File Structure](#file-structure)
-   [Dependencies](#dependencies)
-   [Customization](#customization)
-   [Potential Improvements](#potential-improvements)
-   [License](#license)

## Demo

You can see a working demo of this game at [https://jeopardy-demo.surge.sh/](https://jeopardy-demo.surge.sh/)

## Features

*   **Welcome Screen:** A simple welcome screen with an "Enter Game" button.
*   **Jeopardy Board:** A 6x5 Jeopardy board displayed in an HTML table.
*   **Category Headers:**  Six category headers randomly selected from the data source.
*   **Clue Reveal:** Clicking on a clue ("?") reveals the question.
*   **Answer Reveal:** Clicking on a question reveals the answer.
*   **Restart Game:**  A "Restart" button that reloads new categories and questions.
*   **Data Loading from JSON:** Jeopardy data (categories, questions, and answers) is loaded from a separate `data.json` file.
*   **Random Category Selection:** Randomly selects six categories from the loaded data.

## Installation

1.  **Clone the repository:**

    ```bash
    git clone <repository_url>
    ```

2.  **Navigate to the project directory:**

    ```bash
    cd jeopardy-game
    ```

3.  **(Optional) Set up a local web server:**  You can use a simple Python web server:

    ```bash
    python -m http.server
    ```

    Or use any other web server (e.g., Apache, Nginx). This is generally not needed for local testing of simple HTML/CSS/JS projects, but might be helpful for some environments.

## Usage

1.  Open the `index.html` file in your web browser.
2.  Click the "Enter Game" button on the welcome screen.
3.  Click on a cell with a "?" to reveal the question.
4.  Click on a revealed question to reveal the answer.
5.  Click the "Restart" button to start a new game with new categories and questions.

## Data Source

The game's categories, questions, and answers are stored in the `data.json` file. This file contains a JSON array of category objects, each with a `title` and a `clues` array. Each clue object has a `question` and an `answer` property.

You can modify the contents of `data.json` to customize the questions and categories in the game. Ensure the JSON is valid.

## File Structure
