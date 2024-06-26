# AI-help.in

## Description
This project is a website aimed at providing assistance and resources related to artificial intelligence. It includes registration, login, and other functionalities implemented using Google Apps Script for backend operations.

## Features
- **Registration:** Users can register using their email, username, phone number, designation, company, and password. Duplicate emails prompt a popup notifying the user of the existing account.
- **Password Constraints:** Passwords must include at least 1 capital letter, 1 small letter, 1 digit, and 1 special character.
- **Login:** Registered users can log in using their email and password.
- **OTP Verification:** After registration, users receive an OTP via email for verification.
- **Login Redirect:** Upon successful login, users are redirected to a landing page.
- **Navigation Bar:** The landing page displays a navigation bar with options.
- **User Welcome:** Upon login, users are greeted with a welcome message and their username.
- **Tutorial Video:** A tutorial video is displayed on the landing page.
- **Contact Us:** Users can contact the support team by clicking the "Contact Us" button.
- **Button Highlights:** The register button gets highlighted upon clicking, and when the login button is clicked, it is highlighted while the register button returns to its normal color.
- **Button 1:** Directs users to the home page.
- **Button 2:** Redirects users to google.com.

## How Registration Works
1. **Email Validation:** The user's provided email address is validated to ensure it's not already registered.
2. **Saving User Data:** If the email is unique, the user's registration data including email, username, phone number, designation, company, and password is saved to a spreadsheet.
3. **Generating OTP:** After successful registration, an OTP (One-Time Password) is generated. For demonstration purposes, the OTP is fixed as "6789".
4. **Sending Email with OTP:** The OTP is sent to the user's provided email address for verification.
5. **Redirecting to OTP Page:** Finally, the user is redirected to an OTP verification page.

## How Login Works
1. **Form Submission:** When a user submits the login form, the `doPost()` function in `login.js` is triggered.
2. **Data Retrieval:** The script retrieves the entered email and password from the form submission.
3. **Data Validation:** It then compares the provided email and password with the data stored in a Google Sheets document.
4. **Matching Credentials:** If the entered email and password match with any row in the spreadsheet, the user is redirected to the landing page.
5. **Invalid Credentials:** If no match is found, an error message indicating "Invalid credentials" is returned.

## Google Apps Script Integration
The `doPost()` function interacts with Google Apps Script to handle form submissions and perform data validation. It utilizes the `SpreadsheetApp` service to access and retrieve data from a Google Sheets document.

## Setup
1. Clone this repository to your local machine.
2. Set up a Google Apps Script project and deploy the `doPost()` functions for registration and login.
3. Replace `'1-F2mRYeTd-0Em8fOh1IB7KqwOumsPDWjYUVhYlRn55M'` with the ID of your Google Spreadsheet.
4. Customize the email templates and OTP generation as needed.
5. Host your website on GitHub Pages and update the URLs in the Google Apps Script functions accordingly.

## Usage
1. Open the website.
2. Register with a valid email, ensuring the password meets the specified constraints.
3. Upon duplicate email entry, a popup will notify the user of the existing account.
4. Verify your email using the OTP sent.
5. Log in with your registered email and password.
6. Explore the website features, including the tutorial video.
7. Use the "Contact Us" button to reach out for support.
8. Navigate between pages using the navigation bar.
9. Click "Button 1" to return to the home page.
10. Click "Button 2" to navigate to google.com.

## Technologies Used
- HTML
- CSS
- JavaScript
- Google Apps Script
- Google Sheets

## Contributors
- [Balasubrmani E](https://github.com/DynamicDebugger)
- [Dhivya G](https://github.com/Rallycode)
- [Shreksta R](#)
- [Aravindan L U](#)

## Deployment
The website is deployed using GitHub Pages. We utilized GitHub Pages to host the website directly from the GitHub repository. This deployment method allows for easy sharing and access to the website without the need for additional hosting services.

Deployed Website: [AI-help.in](https://dynamicdebugger.github.io/AI-help.in/)

