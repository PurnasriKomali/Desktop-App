# Desktop-App
## To create a Desktop App using Visual Basic language and Backend using Express and Typescript to replicate the functionality of Google forms.
## Frontend Setup
Open Visual Studio:
Ensure you have Visual Studio installed with Visual Basic support. Create a new Windows Forms App (.NET Framework) project in Visual Basic.

Design the Forms:

Main Form (Form1):
Add two buttons: btnViewSubmissions with the text "View Submissions" and btnCreateNewSubmission with the text "Create New Submission".

CreateSubmissionForm:
Add TextBox controls for Name, Email, Phone, and GitHub Link. Add a Button named btnStopwatch with the text "Toggle Stopwatch". Add a Label to display stopwatch time. Add a Button named btnSubmit with the text "Submit".

ViewSubmissionsForm:
Add TextBox controls to display Name, Email, Phone, GitHub Link, and Stopwatch Time. Add two buttons: btnPrevious with the text "Previous" and btnNext with the text "Next".

Add Event Handlers:
Implement the logic for the stopwatch and form submissions in CreateSubmissionForm. Implement the logic for viewing submissions in ViewSubmissionsForm.

Ensure the following features work:

Create new submissions and view existing submissions.
Keyboard shortcuts for buttons:
Alt + P for Previous
Alt + N for Next
Ctrl + S for Submit
Running the Application
Start the Backend Server:
Navigate to the backend project directory, compile the TypeScript files, and run the server:

bash
Copy code
npx tsc
node dist/index.js
Run the Windows Forms Application:
Open the frontend project in Visual Studio. Build and run the project.

API Endpoints
/ping (GET): Health check endpoint that returns true.
/submit (POST): Submits a new form entry with parameters name, email, phone, github_link, and stopwatch_time.
/read (GET): Retrieves a form entry based on the index parameter.
