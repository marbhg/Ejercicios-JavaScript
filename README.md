# ISTQB ONLINE EXAM
This is an ISTQB Online Exam web project where students can register and take multiple-choice tests. It automatically checks answers, displays scores, and ranks students based on their results.
https://marbhg.github.io/istqb-exam-test/

## BUILD WITH
* ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
* ![JAVASCRIPT](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)


## JIRA PROJECT
[JIRA PROJECT](https://marrqabootcamp.atlassian.net/jira/software/projects/ITE/boards/6)
This project is using JIRA tool for project management and defect traking following agile methodology KANBAB.


## E2E TEST EXECUTION

1. Regression test scenarios are automated using Cypress and Cucumber, and run weekly through continuous integration with GitHub Actions.


## AUTHOR
Marbelis Hugo, QA Engineer
[LinkedIn Profile](www.linkedin.com/in/marbelis-h-)



/* Reset margins and paddings for all elements */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Style for the document body */
body {
    font-family: Arial, sans-serif;
    background: linear-gradient(135deg, #f0f9ff, #e0f7fa); /* Subtle gradient for a dynamic look */
    color: #333; /* Text color */
    display: flex;
    flex-direction: column;
    min-height: 100vh; /* Ensures the body takes at least the full height of the viewport */
}

/* Style for the header */
#header {
    text-align: center;
    padding: 2% 0; /* Top and bottom padding in percentage */
    background-color: #11342c; /* Deep sky blue */
    color: white;
    border-bottom: 5px solid #114533; /* Adds a visual separator */
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

/* Style for the welcome message */
#welcomemessage {
    text-align: center;
    padding: 2% 0; /* Top and bottom padding in percentage */
    font-size: 1.2em;
    color: #00695c;
}

/* Style for the error message */
#errormessage {
    text-align: center;
    padding: 1% 0; /* Top and bottom padding in percentage */
    color: #b81313;
    font-weight: bold;
}

/* Style for grade messages */
#grademessage {
    padding: 1% 0; /* Top and bottom padding in percentage */
    color: #00695c;
    font-style: italic;
    border-top: 2px solid #b2dfdb; /* Adds separation from the question */
    margin-top: 10px;
}

/* Style for final score message */
#gradeexammessage {
    text-align: center;
    font-weight: bold;
    margin-top: 10px;
}

/* Style for the question paragraph */
.question {
    font-weight: bold;
    font-size: 1.1em;
    color: #004f73;
    margin-bottom: 10px;
}

/* Style for sections */
section {
    margin: 2% auto; /* Top and bottom margin in percentage */
    padding: 5%; /* Padding in percentage */
    border-radius: 12px;
    width: 90%;
    background: rgba(255, 255, 255, 0.9); /* Semi-transparent white */
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
    flex-grow: 1; /* Allows sections to grow and occupy available space */
}

/* Style for section headers */
h2 {
    margin-bottom: 15px;
    color: #00796b;
    border-bottom: 2px solid #b2dfdb;
    display: block;
    padding-bottom: 5px;
}

/* Style for all forms */
form {
    display: flex;
    flex-direction: column;
}

/* Style for input fields */
input, select {
    padding: 10px;
    margin-bottom: 10px;
    border: 1px solid #b2dfdb; /* Light green */
    border-radius: 4px;
    transition: border-color 0.3s ease, box-shadow 0.3s ease;
    width: 100%; /* Makes input occupy the full available width */
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

/* Input focus effects */
input:focus, select:focus {
    border-color: #00796b; /* Dark green */
    box-shadow: 0 0 6px rgba(0, 121, 107, 0.5);
    outline: none;
}

/* Style for buttons */
button {
    padding: 12px;
    background-color: #4caf50; /* Light green */
    color: white;
    border: none;
    border-radius: 8px;
    cursor: pointer;
    transition: background-color 0.3s ease, transform 0.2s ease; /* Smooth effect */
    width: 25%; 
    text-align: center;
    margin: 10px auto; /* Vertical spacing and centering */
    display: block; /* Centers buttons */
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}

/* Hover effect for buttons */
button:hover {
    font-weight: bold;
    background-color: #388e3c; /* Dark green */
    transform: scale(1.05); /* Slight enlargement effect */
}

/* Click effect for buttons */
button:active {
    background-color: #3a7e3d; /* Darker green */
    transform: scale(0.95); /* Reduction for click effect */
}

/* Style for the reset button */
button.reset-btn {
    background-color: #175d14; /* Vibrant orange */
    margin-bottom: 30px;
}

/* Reset button hover effect */
button.reset-btn:hover {
    background-color: #29ad4e; /* Darker orange */
}

/* Click effect for the reset button */
button.reset-btn:active {
    background-color: #18531d; 
}

#examform {
    text-align: left;
}

/* Style for radio options */
.radio-option {
    display: grid; /* Grid layout for better alignment */
    grid-template-columns: auto 1fr; /* First column for the button, second for the text */
    align-items: start; /* Ensures text aligns at the top for long labels */
    column-gap: 10px; /* Spacing between button and text */
    margin-bottom: 10px; /* Spacing between options */
    background: #e0f7fa; /* Adds a background for better separation */
    padding: 8px;
    border-radius: 4px;
}

/* Radio input alignment */
.radio-option input[type="radio"] {
    justify-self: start; /* Forces button to align with the left margin */
}

/* Label text alignment */
.radio-option label {
    margin: 0; /* Removes extra margins */
    text-align: left; /* Ensures text is left-aligned */
    white-space: normal; /* Allows line breaks for long text */
}

/* Style for the footer */
footer {
    text-align: center;
    margin-top: 20px;
    padding: 2% 0; /* Top and bottom padding in percentage */
    background-color: #11342c;
    color: white;
    position: relative; /* Ensures footer is correctly positioned */
    bottom: 0; /* Keeps footer at the bottom */
    font-size: 0.9em;
}