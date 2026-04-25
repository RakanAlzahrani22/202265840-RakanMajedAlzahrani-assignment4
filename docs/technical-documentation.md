# Technical Documentation

## Project Overview

This project is an interactive personal portfolio website developed for Assignment 2 in SWE 363. It builds on my Assignment 1 portfolio and adds dynamic behavior, better user feedback, and improved usability using JavaScript, CSS, and browser storage.

The website includes:
- an About section
- a Projects section
- a Contact section

The main technical improvements in this assignment are the interactive project search, form validation, and theme toggle with localStorage.

## Implemented Features

### 1. Live Project Search
A live search feature was added to the Projects section.

#### How it works
- A text input allows the user to type a keyword
- JavaScript listens for the `input` event on the search field
- Each project card contains searchable keywords using a `data-search` attribute
- When the user types, the script checks whether the card matches the search
- Matching projects remain visible
- Non-matching projects are hidden
- A status message tells the user how many projects were found
- If no projects match, an empty-state message appears

#### Why it was added
This feature satisfies the dynamic content requirement because the displayed content changes immediately based on user interaction.

---

### 2. Contact Form Validation
The contact form uses client-side JavaScript validation.

#### Validation rules
- Name must not be empty
- Email must not be empty
- Email must follow a valid email format
- Message must not be empty
- Message must be at least 10 characters long

#### User feedback
- Error messages appear below each form field
- A success message appears when the form is submitted correctly
- The form is frontend-only and does not send data to a server

#### Why it was added
This feature satisfies the data handling and user feedback requirements and improves usability compared to the previous assignment.

---

### 3. Theme Toggle with localStorage
A theme toggle button was added to let the user switch between dark mode and light mode.

#### How it works
- A button toggles the `light-theme` class on the `<body>` element
- CSS applies different colors depending on the active theme
- The selected theme is saved in `localStorage`
- When the page reloads, JavaScript reads the saved value and restores the theme automatically

#### Why it was added
This feature demonstrates basic browser data handling using localStorage and improves the overall user experience.

---

## File Responsibilities

### `index.html`
This file contains the main structure of the website:
- navigation bar
- About section
- Projects section
- Contact section
- search input
- theme toggle button
- validation message placeholders

### `styles.css`
This file contains:
- base page styling
- layout styling
- responsive behavior
- button and card hover effects
- form error and success message styles
- dark and light theme styling
- transition effects for smoother interaction

### `script.js`
This file contains:
- footer year generation
- live project search/filter logic
- contact form validation logic
- success and error feedback handling
- theme toggle logic
- localStorage theme persistence

---

## Responsiveness

The website is responsive and adapts to different screen sizes using CSS media queries.

Responsive behavior includes:
- stacking the About section on smaller screens
- showing project cards in a single column on smaller screens
- keeping buttons flexible on smaller widths

---

## Error Handling and Feedback

The project provides feedback to the user in multiple cases:

- invalid or empty form fields show inline error messages
- a successful form submission shows a success message
- searching with no matching projects shows a “No projects found” message
- the search status updates while the user types

This ensures the user is always informed about what happened.

---

## Technical Challenges Faced

During development, I faced a few issues:
- the project search did not work initially
- the theme toggle did not visually change the page at first
- a CSS brace issue affected layout and some styles

These issues were solved by testing step by step, verifying HTML and JavaScript connections, and correcting the CSS structure.

---

## Limitations

- The contact form does not connect to a backend
- The website currently contains only two projects
- The search feature is simple and designed for a small portfolio

---

## Possible Future Improvements

Possible future improvements include:
- adding more projects
- connecting the contact form to a backend or email service
- improving accessibility further
- adding a Skills section
- deploying the website using GitHub Pages