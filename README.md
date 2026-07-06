# Registration Form

A simple, responsive **Registration Form** built with **HTML, CSS, and JavaScript**, featuring real-time client-side form validation for Name, Email, and Password fields.

## 📋 Description

This project is a lightweight registration form that validates user input before allowing submission. It uses plain JavaScript (no frameworks or libraries) to check each field as the user interacts with it, and displays inline error messages when input doesn't meet the required criteria.

## ✨ Features

- **Name validation** – ensures the name field is not left empty (checked on blur).
- **Email validation** – checks that the email matches a valid email pattern (checked live as the user types).
- **Password validation** – requires a minimum of 8 characters (checked live as the user types).
- **Inline error messages** – errors are displayed directly below each field instead of using intrusive alerts.
- **Submit-time validation** – all fields are re-validated on submit, and the form only proceeds (showing a success alert) if every field passes.
- **Reusable validation functions** – the same `checkName()`, `checkEmail()`, and `checkPassword()` functions are used for both live validation and final submit validation, avoiding code duplication.

## 🗂️ Project Structure

```
registration-form/
├── index.html      # Main HTML file with form markup and JS logic
├── style.css       # Stylesheet for form design and layout
└── README.md       # Project documentation
```

## 🛠️ Tech Stack

- **HTML5** – form structure and semantic markup
- **CSS3** – styling and layout
- **JavaScript (Vanilla JS)** – form validation logic and DOM manipulation

## 🚀 Getting Started

### Prerequisites

You only need a web browser — no build tools or dependencies required.

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/registration-form.git
   ```
2. Navigate into the project folder:
   ```bash
   cd registration-form
   ```
3. Open `index.html` in your browser (double-click it or use a live server extension).

## ✅ Validation Rules

| Field    | Trigger Event | Rule                                      |
|----------|---------------|--------------------------------------------|
| Name     | `blur`        | Cannot be empty or only whitespace         |
| Email    | `input`       | Must match a valid email pattern (`name@domain.xx`) |
| Password | `input`       | Must be at least 8 characters long         |

On clicking **SUBMIT**, all three checks run again. If all pass, an `alert("register completed")` is shown; otherwise, the relevant error messages remain visible.

## 🔮 Possible Improvements

- Add a "confirm password" field to check for matching passwords.
- Style error messages with a distinct color (e.g., red) for better visibility.
- Add password strength indicators (uppercase, number, special character checks).
- Connect the form to a backend/API for actual user registration instead of a simple alert.
- Add success styling/animation instead of a browser `alert()`.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙋 Author

Feel free to fork this project, raise issues, or submit pull requests for improvements!
