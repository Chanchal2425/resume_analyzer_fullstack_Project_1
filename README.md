📊The Resume Analyzer Pro is a full stack web application that helps job seekers optimize their resumes for Applicant Tracking Systems (ATS). Users can upload their PDF resume, paste a job description, and get an instant compatibility score along with matched and missing skills. It's built with React on the frontend and Node.js/Express on the backend


❓The Problem It Solves
"Many companies use ATS software to filter resumes before a human ever sees them. These systems scan for specific keywords and skills mentioned in the job description. If your resume doesn't include those keywords, it gets rejected automatically. My tool helps candidates identify gaps in their resume so they can tailor it for each job application.

✨Frontend Architecture (React)
Component Structure:

The entire application is a single React component called ResumeUploader

It manages several pieces of state using useState:
file – the uploaded PDF file
fileName – just the name for display
jobDesc – the job description text
result – the analysis data from backend
loading – boolean for showing spinner

✨Key UI Sections:

Header – Logo, title, and a "Test Connection" button
Input Section – Two cards side by side:
Job description textarea with character count
File upload area with drag‑and‑drop style

Results Section – Appears after analysis:
Circular progress bar showing ATS score
Stats cards (matched/missing/total skills)
Two skill tag lists (matched in green, missing in red)
Summary text with recommendation
Extracted resume preview

User Experience Features:
Button disabled until both file and JD are provided
Loading spinner during API call
Clear error messages
Color-coded score (green/orange/red)


⚡Backend Architecture (Node.js/Express)
Key Technologies:

Express – web server framework
Multer – handles file uploads
pdf-parse / pdfreader – extract text from PDFs
CORS – allows frontend to communicate
Folder Structure:
server.js – main server file with all endpoints
No separate folders (for simplicity), but in production I'd organize into routes, controllers, services


👏Special Features I Added
1. Multiple PDF Extraction Methods
2. Test Connection Button
3. Skill Variations Handling
4. Visual Score Circle
5. Character Counter

For storage concern and following a good practice insured to upload only the necessary files for user understanding.

📸Snapshot of the project -


<img width="1849" height="917" alt="Screenshot 2025-12-08 110733" src="https://github.com/user-attachments/assets/afb3d6d1-8c5d-4902-ae4a-850ffb3dc5f5" />

<img width="1850" height="918" alt="Screenshot 2025-12-08 110815" src="https://github.com/user-attachments/assets/cdc40748-29f0-45f4-bd2c-52c9a43bdc44" />

<img width="1846" height="898" alt="Screenshot 2025-12-08 110848" src="https://github.com/user-attachments/assets/836e9ec0-97eb-4a04-88fc-5545fb127224" />

<img width="1843" height="912" alt="Screenshot 2025-12-08 110927" src="https://github.com/user-attachments/assets/cb1e1c2a-df62-4079-9e78-2007cf892938" />


# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
