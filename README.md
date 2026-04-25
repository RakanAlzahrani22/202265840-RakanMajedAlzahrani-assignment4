# Assignment 3 – Advanced Portfolio Website

This project is my Assignment 3 submission for SWE 363. It builds on my previous portfolio website from Assignments 1 and 2 by adding advanced functionality, external API integration, stronger state management, and more complex JavaScript logic.

## Project Description

The website is a personal portfolio that introduces me, shows my academic projects, and allows visitors to interact with the page through multiple dynamic features.

This version includes:
- GitHub API integration to display public repositories
- project search, filter, and sort controls
- theme toggle with saved preference
- visitor name personalization with localStorage
- validated contact form with user feedback

## Features

### 1. GitHub API Integration
- Loads my latest public GitHub repositories
- Displays repository name, description, language, and link
- Shows loading and error feedback

### 2. Project Search, Filter, and Sort
- Search projects by keyword
- Filter projects by category
- Sort projects alphabetically
- Shows an empty-state message when no projects match

### 3. State Management
- Theme preference is saved using `localStorage`
- Visitor name is saved using `localStorage`
- Greeting updates dynamically based on saved name

### 4. Form Validation
- Validates empty fields
- Checks email format
- Ensures the message is long enough
- Displays inline error messages and success feedback

## Technologies Used

- HTML5
- CSS3
- JavaScript
- GitHub REST API
- localStorage
- Git and GitHub

## Project Structure

```text
id-name-assignment3/
├── README.md
├── index.html
├── css/
│   └── styles.css
├── js/
│   └── script.js
├── assets/
│   └── images/
├── docs/
│   ├── ai-usage-report.md
│   └── technical-documentation.md
└── .gitignore