# Assignment 4 – Personal Web Application

This project is my final submission for SWE 363. It brings together the work completed in Assignments 1, 2, and 3 into a polished personal web application that demonstrates responsive design, JavaScript interactivity, API integration, state management, and professional presentation.

## Project Overview

This website is a personal portfolio web application that introduces me, showcases my academic projects, and demonstrates the front-end development skills I built throughout the course.

The application includes:
- a responsive personal portfolio layout
- interactive project search, filter, and sort
- GitHub API integration for displaying public repositories
- theme persistence using `localStorage`
- visitor name personalization using `localStorage`
- contact form validation with user feedback
- a project details modal for a more polished experience

## Main Features

### 1. Interactive Portfolio Sections
- About section with personal introduction
- Projects section with featured academic work
- GitHub section with live repository data
- Contact section with validation and feedback

### 2. Project Search, Filter, and Sort
Users can:
- search projects by keyword
- filter projects by category
- sort projects alphabetically
- view an empty-state message when nothing matches

### 3. GitHub API Integration
The website fetches public repositories from GitHub and displays:
- repository name
- description
- main language
- link to the repository

The interface also provides:
- loading feedback
- error feedback if the API request fails

### 4. State Management
The application remembers:
- the selected light or dark theme
- the visitor’s saved name

This is handled using `localStorage`.

### 5. Contact Form Validation
The contact form:
- checks for empty fields
- validates email format
- enforces a minimum message length
- displays inline error messages
- shows a success message after valid submission

### 6. Final Innovation Feature
A project details modal was added so visitors can open a focused view of project information without leaving the page. This improves the user experience and makes the application feel more professional.

## Technologies Used

- HTML5
- CSS3
- JavaScript
- GitHub REST API
- localStorage
- Git and GitHub

## Project Structure

```text
id-name-assignment4/
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
├── presentation/
│   ├── slides.pdf
│   └── demo-video.mp4
└── .gitignore