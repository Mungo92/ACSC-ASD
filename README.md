# ACSC-ASD
Export Functionality:

The exportToPDF function has been updated to properly include the company logo in the PDF. Since jsPDF requires the image in Base64 format, I've added an async function getBase64ImageFromURL to fetch and convert the image.
The function generates a PDF with the following structure:
Front Page: Contains your company logo, the title, user details, and the compliance score.
Checklist Responses: Lists all questions and the user's answers.
To-Do List: A separate page that lists remediation tasks for all "No" answers.
Back Page: Contains your contact details.
Professional Design:

The PDF uses consistent fonts, sizes, and alignment to ensure a professional and premium appearance.
Text wrapping is handled to prevent content from overflowing the page.
Additional Features:

The Popup Form collects and stores user details in localStorage. The form is displayed until the user provides the required information.
The Background Blur effect is applied when the popup form is active.
The Save Progress button allows users to save their current checklist state.
The Reset button clears all data, including user details, and brings back the popup form.
The Glossary Modal provides definitions for terms used in the checklist.
How to Use the Code:

Copy and Paste: Copy the entire code and paste it into an .html file on your computer or server.

Open in Browser: Open the HTML file in a modern web browser (e.g., Chrome, Firefox, Edge).

Enter Details: When the page loads, the popup form will appear. Fill in all the fields and click "Next".

Complete the Checklist: Go through each question and select "Yes" or "No".

View Compliance Score: The compliance score and progress bar will update automatically.

View To-Do List: Based on your "No" answers, the to-do list will populate with remediation tasks.

Save Progress: Click "Save Progress" to save your answers locally in the browser.

Export to PDF: Click "Export" to download a professionally formatted PDF of your responses and to-do list.

Reset: Click "Reset" to clear all data and start over.

Dependencies:

jsPDF: A JavaScript library to generate PDFs.
html2canvas: Used to handle image conversion for the logo in the PDF.
Customization:

Logo: Ensure the logoSrc variable points to the correct URL of your logo. If you wish to use a local image, you'll need to adjust the code accordingly.

Contact Details: Update the contact details in the "Back Page with Contact Details" section to reflect any changes.

Testing:

Local Testing: When testing locally, some browsers may block local file access for security reasons. If you encounter issues with the logo not appearing, consider testing on a local server or ensure that CORS policies are not blocking the image fetch.

Browser Compatibility: The code should work on modern browsers that support localStorage and ES6 JavaScript features.

Let me know if you have any questions or need further assistance!
