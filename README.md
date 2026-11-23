# ReadmitIQ – 30-Day Hospital Readmission Risk Prediction System

## Project Overview

**ReadmitIQ** is a web-based hospital readmission risk assessment and analytics application developed to demonstrate how healthcare information can be used to estimate the likelihood of a patient being readmitted within 30 days after discharge.

The application provides an interactive interface for entering patient details, generating simulated readmission risk scores, managing demonstration patient records, and visualizing risk patterns through dashboards.

This project demonstrates the integration of healthcare analytics concepts with modern frontend web development.

> **Disclaimer:** ReadmitIQ is an educational prototype. Its prediction scores are generated using a handcrafted logistic scoring formula, not a trained or clinically validated machine learning model. It must not be used for real patient care or medical decisions.

## Objectives

- Develop an interactive hospital readmission risk prediction interface.
- Analyze patient information and associated risk factors.
- Classify estimated readmission risk into different categories.
- Visualize patient statistics and risk distributions.
- Provide a simple and user-friendly healthcare analytics dashboard.
- Demonstrate the potential of data-driven healthcare applications.

## Key Features

### 1. Dashboard
Displays an overview of patient records, risk statistics, and visual analytics to help users understand the distribution of estimated readmission risk.

### 2. Risk Prediction
Allows users to enter patient information, including:

- Age and length of hospital stay
- Previous hospital admissions
- Medical conditions such as diabetes, hypertension, heart disease, chronic kidney disease, COPD, asthma, cancer, obesity, and others
- Admission type and source
- Diagnosis and discharge destination
- ICU admission and surgical history

The application calculates an illustrative risk percentage and displays the corresponding risk category.

### 3. Patient Records
Provides an interface to view and search demonstration patient records and their estimated readmission risk scores.

### 4. Model Calibration
Presents educational information about prediction confidence, calibration, and the importance of evaluating risk models.

The application does not perform actual statistical calibration against clinical outcome data.

### 5. Reports and Analytics
Displays charts and summaries for understanding simulated patient risk patterns.

## Technologies Used

| Technology | Purpose |
|---|---|
| React.js | Frontend user interface |
| JavaScript | Application logic and risk calculations |
| Vite | Development and production build tool |
| Tailwind CSS | Styling and responsive layout |
| Recharts | Charts and data visualization |
| Lucide React | Interface icons |
| GitHub | Source code version control |
| Vercel | Website deployment |

## System Workflow

```text
Patient Information
        |
        v
Input Validation
        |
        v
Risk Factor Processing
        |
        v
Simulated Logistic Risk Formula
        |
        v
Risk Percentage Calculation
        |
        v
Risk Category Classification
        |
        v
Dashboard and Reports
```

## Risk Prediction Methodology

ReadmitIQ uses a handcrafted logistic scoring approach to demonstrate how multiple patient characteristics can be combined into an estimated risk percentage.

The basic logistic function is:

```text
P = 1 / (1 + e^(-z))
```

Where:

- `P` represents the estimated probability.
- `z` is a weighted combination of selected risk factors.
- `e` is Euler's number.

The application converts the resulting value into a percentage and assigns a risk category.

The weights are illustrative and have not been estimated from clinical training data.

## Project Structure

```text
hospital-readmission/
├── public/
├── src/
│   ├── App.jsx
│   ├── main.jsx
│   └── index.css
├── index.html
├── package.json
├── package-lock.json
├── vite.config.js
├── .gitignore
└── README.md
```

## Installation and Setup

### Prerequisites

Install:

- Node.js
- npm
- Visual Studio Code
- Git

### Clone the Repository

```bash
git clone https://github.com/PriyaGuggilla/hospital-readmission-prediction.git
```

### Open the Project Folder

```bash
cd hospital-readmission-prediction
```

### Install Dependencies

```bash
npm install
```

### Start the Development Server

```bash
npm run dev
```

Open the local address displayed in the terminal, typically:

```text
http://localhost:5173
```

### Create a Production Build

```bash
npm run build
```

The production files are generated in the `dist` folder.

## Deployment

The project is designed to be deployed using **Vercel**.

Recommended deployment settings:

| Setting | Value |
|---|---|
| Framework | Vite |
| Build Command | `npm run build` |
| Output Directory | `dist` |

## Testing

The application can be tested using synthetic patient records and sample inputs.

Suggested test scenarios include:

1. Entering valid patient information.
2. Checking whether changes to risk factors affect the calculated score.
3. Verifying risk category classification.
4. Searching patient records.
5. Navigating between dashboard sections.
6. Checking chart rendering and responsive layouts.
7. Confirming successful production builds.

## Limitations

- The model is not trained using real hospital datasets.
- Risk scores are not clinically validated.
- Prediction calibration has not been established using observed readmission outcomes.
- The application is primarily a frontend demonstration.
- Patient records are synthetic and are not a substitute for a secure clinical database.
- The application is not intended for diagnosis, treatment, or clinical decision-making.

## Future Enhancements

- Train a machine learning model using appropriately authorized, de-identified healthcare datasets.
- Evaluate model discrimination and calibration.
- Integrate a secure backend and database.
- Implement role-based authentication.
- Add model monitoring and explainability features.
- Provide downloadable analytics reports.
- Improve accessibility and mobile responsiveness.

## References

1. React Documentation — https://react.dev/
2. Vite Documentation — https://vite.dev/
3. Tailwind CSS Documentation — https://tailwindcss.com/docs
4. Recharts — https://recharts.org/
5. Vercel Documentation — https://vercel.com/docs
6. Scikit-learn: Probability Calibration — https://scikit-learn.org/stable/modules/calibration.html

## Project Repository

https://github.com/PriyaGuggilla/hospital-readmission-prediction

---

**Project Name:** ReadmitIQ – 30-Day Hospital Readmission Risk Prediction System

**Project Type:** Academic Web Development and Healthcare Analytics Demonstration

**Developed Using:** React, JavaScript, Vite, Tailwind CSS, and Recharts

**Purpose:** Educational and academic demonstration only.

