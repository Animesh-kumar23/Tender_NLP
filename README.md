Tender & Proposal Compliance Checker

Description

The Tender & Proposal Compliance Checker is a ReactJS-based web application that evaluates whether a submitted proposal fulfills all criteria outlined in a tender document. The application uses PDF.js for PDF parsing and Compromise NLP for text analysis. It supports dynamic section detection and condition validation, ensuring comprehensive compliance checks.

Features
Parse and extract text from multi-page tender and proposal PDF files.
Identify and validate tender conditions, including:
Eligibility criteria
Compliance conditions
Special conditions
Local content requirements
Use a Web Worker to process the documents without blocking the UI.
Outputs a summary of compliance status and any unmet conditions.
Technologies Used
ReactJS: Frontend framework
PDF.js: For parsing and extracting text from PDF files
Compromise NLP: For natural language processing and section detection
Web Workers: For efficient background processing of text analysis

Installation

Prerequisites

Node.js (>=16.x)
npm or yarn
Steps
Clone the repository:
Copy code
git clone https://github.com/your-username/tender-proposal-checker.git
cd tender-proposal-checker

Install dependencies:

npm install
Start the development server:

npm start
Usage
Upload the tender PDF and proposal PDF using the provided file inputs.
Click the Check Compliance button.
View the compliance results, which include:
A summary of whether all conditions are satisfied.
A detailed list of unsatisfied conditions (if any).

File Structure
php
tender-proposal-checker/
├── public/
├── src/
│   ├── components/
│   │   ├── TenderProposalChecker.jsx  # Main React component
│   ├── App.js                         # Entry point for the app
│   ├── index.js                       # Renders the React app
├── package.json                       # Project metadata and dependencies
└── README.md                          # Project documentation

How It Works

PDF Parsing:

Uses PDF.js to extract text from the uploaded PDF files.
Text Processing:
Employs Compromise NLP to analyze the extracted text, detect sections, and evaluate conditions.
Background Processing:
Delegates the compliance checking to a Web Worker for smooth performance.

Results:

Displays whether the proposal meets all tender requirements.
Lists unsatisfied conditions (if any).
Libraries and Tools
ReactJS
PDF.js
Compromise NLP
Web Workers
Example Output

Input:

Tender Document:
Specifies eligibility, compliance, and local content requirements.
Proposal Document:
Details the bidder's credentials and certifications.
Output:
If all conditions are met:
plaintext

All conditions are satisfied.
If some conditions are unmet:
plaintext

Some conditions are not satisfied.
Unsatisfied Conditions:
- Section: Special Conditions, Condition: replacement of all lighting equipment is mandatory.
- Section: Local Content, Condition: local content requirement not met.
Contributing
Contributions are welcome! If you'd like to contribute:

Fork the repository.
Create a new branch (git checkout -b feature/your-feature).
Commit your changes (git commit -m "Add your feature").
Push to the branch (git push origin feature/your-feature).
Open a Pull Request.


Contact
Author: Animesh Kumar
Email: animeshkumar.bgs@gmail.com
GitHub Repository: https://github.com/your-username/tender-proposal-checker
