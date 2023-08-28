# README - HTML Form Integration with Google Form

This README provides instructions on how to integrate an HTML form with a Google Form and customize it accordingly. The HTML form will be linked to a Google Form for data submission. The process involves extracting input field names from the Google Form and updating the HTML form code with the appropriate input field names.

## Prerequisites

- Basic knowledge of HTML and web development.
- A Google account to create and manage Google Forms.

## Instructions

1. **Create a Google Form:**
   - Log in to your Google account.
   - Go to Google Forms (forms.google.com).
   - Create a new form or choose an existing one.

2. **Inspect Input Fields:**
   - Open the Google Form.
   - Right-click on each input field (textboxes, dropdowns, etc.).
   - Select "Inspect" or "Inspect Element" to open the browser developer tools.
   - Locate the `name` attribute of the input field. This attribute holds the unique name of the input field. Make a note of these names for each input you want to include in your HTML form.

3. **Update HTML Form Code:**
   - Open the HTML file where you want to integrate the Google Form.
   - Locate the `<form>` tag within your HTML code.
   - In the `action` attribute of the `<form>` tag, replace the placeholder link with the link to your Google Form. The `action` attribute specifies where the form data will be submitted.
   - For example: `<form action="https://docs.google.com/forms/d/e/YourFormID/formResponse" method="POST">`

4. **Update Input Fields:**
   - Inside the `<form>` tag, locate the input fields you want to include.
   - For each input field, update the `name` attribute with the corresponding input field name you obtained from the Google Form.
   - Example: `<input type="text" name="entry123456789">`

5. **Placeholder Values:**
   - To make the form user-friendly, provide placeholders for each input field that indicate what information is expected.
   - Update the `placeholder` attribute of each input field with a descriptive placeholder value.
   - Example: `<input type="text" name="entry123456789" placeholder="Your Name">`

6. **Submit Button:**
   - Ensure your HTML form has a submit button to allow users to submit their data.
   - Customize the button's appearance and text to match your design and intent.

7. **Testing:**
   - Save your HTML file and open it in a web browser.
   - Fill out the form and click the submit button to test the data submission to the Google Form.

8. **Collect Data:**
   - Data submitted through your HTML form will now be collected in your linked Google Form's response spreadsheet.

## Note
- Keep in mind that Google Forms and its structure may change over time, so the instructions provided here are based on the state of Google Forms as of my last knowledge update in September 2021.

Always double-check the steps and consult Google's official documentation for any updates or changes that might have occurred since then.
