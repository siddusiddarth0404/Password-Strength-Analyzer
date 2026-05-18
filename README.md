# Password Strength Evaluator

A lightweight, front-end interactive tool built with vanilla HTML, CSS, and JavaScript that evaluates password strength in real-time. It provides immediate visual feedback, a checklist of security requirements, and a built-in secure password generator.

## Features

* **Real-Time Evaluation:** Calculates password strength instantly as the user types.
* **Visual Strength Meter:** A dynamic progress bar that categorizes passwords into four levels: Weak, Moderate, Strong, and Very Strong.
* **Dynamic Checklist:** A visual list that updates dynamically (✗ to ✓) as the user meets specific character requirements (length, uppercase, lowercase, numbers, symbols).
* **Compromised Password Simulation:** Checks input against a hardcoded list of commonly reused or breached passwords (e.g., "123456", "password"). If a match is found, the score instantly drops to zero and displays a warning.
* **Secure Password Generator:** A one-click button to generate a fully randomized, 16-character password that guarantees inclusion of all required character types.
* **Visibility Toggle:** Allows users to show or hide the password they are typing.

## Technologies Used

* **HTML5:** Standard semantic markup.
* **CSS3:** Custom styling for the interface, including transitions for the strength meter and responsive design for mobile viewing.
* **JavaScript (ES6):** Handles DOM manipulation, regular expression checking, strength scoring algorithms, and password generation. No external libraries or frameworks are required.

## Installation and Usage

This project is entirely client-side and contained within a single file. No server setup, build processes, or package managers are required.

1. Create a new file named `index.html`.
2. Copy the provided HTML/CSS/JS code and paste it into the file.
3. Save the file.
4. Double-click `index.html` to open it in any modern web browser (Chrome, Firefox, Safari, Edge).

## Customization

You can easily customize the tool by editing the JavaScript section:

* **Update Compromised Passwords:** Add more strings to the `compromisedPasswords` array to expand the "database" of forbidden passwords.
* **Tweak Requirements:** Modify the `if` statements containing the Regular Expressions to change what constitutes a strong password (e.g., increasing the minimum length requirement).
* **Adjust Generator Length:** Change the loop limit in the `generateBtn` event listener to generate passwords longer or shorter than 16 characters.
