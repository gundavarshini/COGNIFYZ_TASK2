# Cognifyz Level 1 - Task 2

## Inline Styles, Basic Interaction, and Server-Side Validation

### Overview

This project is developed as part of the **Cognifyz Technologies Full Stack Development Internship – Level 1, Task 2**.

The objective of this task is to extend the basic web application developed in Task 1 by introducing **advanced HTML forms, inline styling, client-side interaction, server-side validation, and temporary server-side data storage**.

The application demonstrates how user input can be validated on both the client and server sides before being processed and stored temporarily.



## Task Objective

The main objectives of this task are:

- Extend the HTML structure with more complex forms.
- Add inline CSS styles to improve the user interface.
- Implement basic user interactions using JavaScript.
- Perform client-side form validation.
- Implement server-side validation using Node.js and Express.js.
- Store validated form data temporarily on the server.
- Display appropriate success or validation messages to the user.



## Technologies Used

- **HTML5** - Used to create the form structure and user interface.
- **CSS3** - Used for styling and improving the appearance of the application.
- **JavaScript** - Used for client-side interaction and form validation.
- **Node.js** - Used as the server-side runtime environment.
- **Express.js** - Used for server creation, routing, and request handling.
- **EJS** - Used for server-side rendering and dynamically displaying data.
- **npm** - Used for dependency management.

---

## Key Features

### 1. Enhanced HTML Form

The application contains an extended form with multiple input fields to collect user information.

### 2. Inline Styling

Inline CSS styles are used to customize elements such as:

- Text
- Buttons
- Input fields
- Form sections
- Backgrounds
- Layout elements

### 3. Client-Side Validation

JavaScript is used to validate user input before the form is submitted to the server.

This helps identify invalid or incomplete data immediately.

### 4. Server-Side Validation

The Express.js server validates the submitted data before accepting it.

Server-side validation ensures that invalid data cannot bypass the validation performed in the browser.

### 5. Temporary Server-Side Storage

Validated form data is stored temporarily on the server for demonstration purposes.

No permanent database is required for this task.

### 6. Dynamic Response

EJS is used to dynamically generate the response page based on the submitted and validated information.


## Application Workflow


        User Opens Application
                 |
                 v
          HTML Form Displayed
                 |
                 v
          User Enters Data
                 |
                 v
       Client-Side Validation
                 |
          +------+------+
          |             |
       Invalid        Valid
          |             |
          v             v
    Show Error       Submit Form
                        |
                        v
               Express.js Server
                        |
                        v
               Server-Side Validation
                        |
                 +------+------+
                 |             |
              Invalid        Valid
                 |             |
                 v             v
            Error Page    Temporary Storage
                               |
                               v
                         EJS Rendering
                               |
                               v
                         Result Page
                         
Project Structure

Level1_Task2/
│
├── node_modules/
│
├── public/
│   └── style.css
│
├── views/
│   ├── index.ejs
│   ├── result.ejs
│   └── error.ejs
│
├── package.json
├── package-lock.json
├── server.js
└── README.md

File Description

| File/Folder         | Description                                   |
| ------------------- | --------------------------------------------- |
| `server.js`         | Main Node.js and Express.js server            |
| `views/index.ejs`   | Contains the user input form                  |
| `views/result.ejs`  | Displays successfully submitted data          |
| `views/error.ejs`   | Displays validation errors                    |
| `public/style.css`  | Contains CSS styles                           |
| `package.json`      | Stores project configuration and dependencies |
| `package-lock.json` | Locks dependency versions                     |
| `node_modules/`     | Contains installed npm packages               |
| `README.md`         | Project documentation                         |


Validation Process

The application uses two levels of validation.

Client-Side Validation

Client-side JavaScript checks the form before sending the request to the server.

For example:

Required fields
Valid email format
Minimum input length
Valid user input

If the input is invalid, an error message is displayed without submitting the form.

Server-Side Validation

After the form is submitted, the Express.js server performs another validation.

The server checks whether:

Required fields are present.
Submitted values are valid.
The input meets the required conditions.

Only validated data is temporarily stored and processed.

Installation and Setup

Step 1: Clone the Repository
git clone <YOUR_GITHUB_REPOSITORY_URL>

Step 2: Navigate to the Project
cd Level1_Task2

Step 3: Install Dependencies
npm install

If Express and EJS are not installed:
npm install express ejs

Step 4: Start the Server
node server.js

Step 5: Open the Application
Open the following URL in your browser:
http://localhost:3000

Example Application Flow

->Open the application in a web browser.
->Enter the required information in the form.
->Click the Submit button.
->JavaScript performs client-side validation.
->If valid, the data is sent to the Express.js server.
->The server performs server-side validation.
->Valid data is temporarily stored.
->EJS dynamically generates the response page.
->The submitted information is displayed to the user.

Learning Outcomes

Through this task, I gained practical experience in:

->Creating advanced HTML forms.
->Applying inline CSS styles.
->Implementing JavaScript-based client-side validation.
->Understanding server-side validation.
->Handling form submissions using Express.js.
->Creating Express.js routes.
->Processing HTTP POST requests.
->Using EJS for dynamic server-side rendering.
->Temporarily storing data on the server.
->Understanding frontend and backend interaction.
->Improving user experience through validation and feedback.

Screenshots
Home / Registration Page
<img width="798" height="667" alt="image" src="https://github.com/user-attachments/assets/6c1fc187-11b9-4a9d-96ed-4c95f2fbb2bf" />
<img width="794" height="590" alt="image" src="https://github.com/user-attachments/assets/3ee8fd1a-84fc-4ad2-a0aa-fbc92c9637e0" />



Validation / Result Page

<img width="743" height="721" alt="image" src="https://github.com/user-attachments/assets/97906231-a142-4473-b843-db2cb156c134" />

Future Enhancements

The application can be further enhanced by adding:

1.Database integration using MySQL or MongoDB.
2.User authentication and authorization.
3.Password encryption.
4.Improved responsive design.
5.REST API integration.
6.Permanent data storage.
7.Advanced form validation.
8.Better error handling.
9.Session management.
10.Improved UI/UX.
11.Internship Details

Organization: Cognifyz Technologies

Program: Full Stack Development Internship
Level: Level 1 - Beginner
Task: Task 2 - Inline Styles, Basic Interaction, and Server-Side Validation

Author

Varshini Reddy

GitHub: <gundavarshini>

Conclusion

This project demonstrates the implementation of interactive HTML forms with both client-side and server-side validation.
By combining HTML, CSS, JavaScript, Node.js, Express.js, and EJS, the application provides a basic example of full-stack web development and demonstrates how data flows from the frontend to the backend and is dynamically rendered back to the user.
