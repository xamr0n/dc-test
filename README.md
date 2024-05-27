# README for "5 Random Questions" Quiz Webpage

## Overview

This project is a simple HTML, CSS, and JavaScript-based quiz application named "5 Random Questions." It generates a random set of five questions from a pool of predefined questions, displays them to the user one at a time, and calculates the score based on the user's answers.

## Table of Contents

1. [Features](#features)
2. [Structure](#structure)
3. [Styling](#styling)
4. [Functionality](#functionality)
5. [Installation](#installation)
6. [Usage](#usage)
7. [Customization](#customization)
8. [Credits](#credits)

## Features

- Randomly selects 5 questions from a pool of predefined questions.
- Displays one question at a time with multiple-choice answers.
- Calculates and displays the score at the end of the quiz.
- Provides a reset button to retake the quiz with a new set of random questions.
- Responsive design for different screen sizes.

## Structure

The project consists of the following main components:

1. **HTML**: The structure of the webpage.
2. **CSS**: The styling of the webpage.
3. **JavaScript**: The functionality of the quiz application.

### HTML

The HTML file includes:
- A `div` with the class `card` for a home link.
- A main `h1` heading for the quiz title.
- A `div` with the class `container` that contains:
  - A secondary `h1` for the test name.
  - `div` elements for displaying questions and answers.
  - A submit button for submitting answers.
  - A `div` for displaying the score.

### CSS

Inline CSS styles provide:
- Basic styling for the body, container, and elements within the container.
- Hover effects for buttons to enhance user experience.

### JavaScript

The `app.js` script handles:
- Randomly selecting questions from the predefined pool.
- Displaying questions and answers.
- Handling user interactions (answer selection and submission).
- Calculating and displaying the score.
- Resetting the quiz for a new attempt.

## Styling

The page is styled using both an external CSS file (`styles.css`) and inline CSS within the HTML document. The styling aims to create a clean and professional look with the following features:
- Background color: `#eee`
- Text color: `#666`
- Rounded corners and shadows for the container and buttons.
- Font family: Candara, sans-serif.
- Hover effects for interactive elements like buttons.

## Functionality

### Random Question Selection

The `getRandomQuestions` function selects 5 random questions from the `allQuestions` array.

### Displaying Questions

The `showQuestion` function displays the current question and its multiple-choice answers.

### Handling User Answers

The `submitAnswer` function checks the selected answer, updates the score, and moves to the next question. If all questions are answered, it displays the final score.

### Resetting the Quiz

The `resetQuiz` function resets the quiz, allowing the user to retake it with a new set of random questions.

## Installation

To run this project, simply clone or download the repository and open the `index.html` file in a web browser.

## Usage

1. Open the `index.html` file in your preferred web browser.
2. The quiz will start automatically with a random set of 5 questions.
3. Select an answer for each question and click the "Submit" button.
4. After submitting all answers, the score will be displayed.
5. Click the "Reset" button to retake the quiz with a new set of questions.

## Customization

You can customize the quiz by editing the questions in the JavaScript section of the HTML file. Each question object contains a `question` string and an `answers` array. The `answers` array contains objects with `text` and `correct` properties.

## Credits

This project uses the following resources:

- [Font Awesome](https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css) for icons.
- Inspiration and guidance from various online tutorials and code examples.

Example:

```javascript
{
  question: "What is the primary responsibility of a Project Document Controller?",
  answers: [
    { text: "Managing project finances", correct: false },
    { text: "Coordinating project meetings", correct: false },
    { text: "Ensuring proper documentation control", correct: true },
    { text: "Handling construction equipment", correct: false }
  ]
}


