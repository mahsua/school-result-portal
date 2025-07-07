# School Result Portal

## Live Demo

Experience the live application here: [School Result Portal](https://mahsua.github.io/school-result-portal/)

## Project Description

The School Result Portal is a user-friendly web application designed to allow students to view their academic results online. Students can enter their Roll Number, select their Class, and provide their Enrollment Number to retrieve and display their detailed results, including subject-wise marks, percentage, grade, and pass/fail status. The application is designed with a clean, attractive UI and offers a convenient print option for results.

## Features

* **Dynamic Result Retrieval:** Fetch and display student results based on Roll Number, Class, and Enrollment Number.
* **Attractive User Interface:** A clean, modern design with a focused color palette (blue, pink, green) for an appealing look.
* **Conditional Print Button:** A print button appears only when a result is successfully displayed, allowing students to easily print their mark sheets.
* **Clear Messaging:** Provides informative messages for loading states, errors (e.g., student not found), and successful operations.
* **Organized Data Display:** Presents student details and subject marks in a well-structured and readable format, with optimized spacing for clarity.
* **Responsive Design:** Adapts to different screen sizes for a consistent experience on desktops, tablets, and mobile devices.

## How to Use (Local Setup)

To run this project locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/mahsua/school-result-portal.git](https://github.com/mahsua/school-result-portal.git)
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd school-result-portal
    ```
3.  **Prepare Data (if not already present):**
    Ensure you have your student data in JSON files (e.g., `class_1.json`, `class_2.json`) inside a `data/` directory at the root of your project. The `index.html` file references these paths. Example structure for `data/class_1.json`:
    ```json
    [
      {
        "Student Name": "Amit Patel",
        "Student Roll Number": 101,
        "Enrollment Number": "ENR001AP",
        "Mark Obtained (Math)": 85,
        "Mark Obtained (Science)": 90,
        "Mark Obtained (English)": 75,
        "Percentage": 83.33,
        "Grade": "A",
        "Pass/Fail": "Pass"
      },
      {
        "Student Name": "Priya Sharma",
        "Student Roll Number": 102,
        "Enrollment Number": "ENR002PS",
        "Mark Obtained (Math)": 60,
        "Mark Obtained (Science)": 65,
        "Mark Obtained (English)": 70,
        "Percentage": 65,
        "Grade": "C",
        "Pass/Fail": "Pass"
      }
    ]
    ```
4.  **Serve the application using a local web server:**
    Due to browser security restrictions (`CORS` policy, `file://` protocol), you cannot directly open `index.html` in your browser for the application to function correctly. You need a simple local web server.

    If you have Python installed, you can run:
    ```bash
    python -m http.server 8000
    ```
    Then, open your web browser and go to: `http://localhost:8000/`

    Alternatively, you can use other local server solutions like Live Server VS Code extension, Node.js `http-server`, etc.

## Project Structure
```
├── index.html            # Main application file
├── data/                 # Directory for storing student result JSON files
│   ├── class_1.json      # Example data for Class 1
│   └── class_2.json      # Example data for Class 2
└── README.md             # This file
```

# Technologies Used

* **HTML5:** For the structure of the web page.
* **CSS3:** For styling the application, including custom CSS variables for theme management.
* **Tailwind CSS (CDN):** A utility-first CSS framework for rapid UI development.
* **JavaScript (Vanilla JS):** For handling form submissions, fetching data, rendering results, and managing UI interactivity.

## Contributing

Feel free to fork the repository and contribute to this project. Pull requests are welcome!
