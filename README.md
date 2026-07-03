# Resume Analyzer

Resume Analyzer is a full-stack web application that uses Artificial Intelligence to analyze resumes and provide meaningful insights, including skill extraction, resume evaluation, improvement suggestions, and relevant job recommendations. The application also includes secure user authentication with email verification, password reset, and Google Sign-In.

---

## Features

* AI-powered resume analysis using Google Gemini
* Resume upload and analysis
* Resume improvement suggestions
* Skill extraction from resumes
* Resume evaluation and feedback
* Job recommendations using Adzuna API
* JWT-based authentication
* Email verification using Brevo
* Password reset via email
* Google OAuth 2.0 Login
* Previous resume analysis history
* Responsive React-based user interface

---

## Tech Stack

### Frontend

* React.js
* HTML5
* CSS3
* JavaScript
* Vite

### Backend

* Java
* Spring Boot
* Spring Security
* JWT Authentication
* Maven

### Database

* MySQL

### AI & APIs

* Google Gemini AI
* Adzuna Job Search API
* Brevo Email API
* Google OAuth 2.0

---

## Project Structure

```text
Resume-Analyser
│
├── frontend src/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── vite.config.js
│
├── src/
│   ├── main/
│   │   ├── java/
│   │   ├── resources/
│   │   └── static/
│   └── test/
│
├── Dockerfile
├── pom.xml
├── render.yaml
└── README.md
```

---

## Prerequisites

Before running the application, ensure you have installed:

* Java 17 or above
* Maven
* Node.js
* MySQL
* Git

---

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/prasad0443/Resume-Analyser.git
```

### 2. Open the Project

Open the project in IntelliJ IDEA, Eclipse, or VS Code.

Allow Maven to download all required dependencies.

---

## Configure `application.properties`

Configure the following credentials before running the application.

### MySQL

```properties
spring.datasource.url=YOUR_DATABASE_URL
spring.datasource.username=YOUR_DATABASE_USERNAME
spring.datasource.password=YOUR_DATABASE_PASSWORD
```

### Google OAuth

```properties
spring.security.oauth2.client.registration.google.client-id=YOUR_GOOGLE_CLIENT_ID
spring.security.oauth2.client.registration.google.client-secret=YOUR_GOOGLE_CLIENT_SECRET
```

### Google Gemini AI

```properties
genKey=YOUR_GEMINI_API_KEY
```

### Brevo Email API

```properties
apiKey=YOUR_BREVO_API_KEY
```

### Adzuna API

```properties
application-id=YOUR_ADZUNA_APP_ID
application-api-key=YOUR_ADZUNA_API_KEY
```

### JWT

```properties
jwt-key=YOUR_SECRET_KEY
```

---

## Running the Project

### Backend

Run the Spring Boot application:

```text
ResumeAnalyserApplication.java
```

The application starts at:

```text
http://localhost:8080/
```

---

## Frontend Development

Run the React frontend separately during development:

```bash
cd "frontend src"
npm install
npm run dev
```

---

## Production Build

Generate the React production build:

```bash
cd "frontend src"
npm run build
```

Copy the generated files from the `dist` folder into:

```text
src/main/resources/static/
```

Replace:

* `index.html`
* `assets/`

---

## Screenshots

Add screenshots of:

* Home Page
* Login Page
* Resume Upload
* Resume Analysis Results
* Previous Analysis History

---

## Important Notes

* The application currently uses Google Gemini AI for resume analysis.
* Email functionality is implemented using the Brevo API.
* Job recommendations are powered by the Adzuna API.
* If an API provider changes or deprecates a service, update the corresponding service implementation accordingly.

---

## Future Improvements

* ATS Resume Score
* Resume vs Job Description Matching
* DOCX Resume Support
* AI Interview Question Generator
* Download Analysis as PDF
* Dashboard Analytics

---

## Acknowledgements

This repository is based on the open-source Resume Analyzer project created by Mohamed Imran. It is maintained for educational purposes, learning, and future enhancements.

Original Repository:
https://github.com/Mohamed-Imran-12/Resume-Analyser

---

## License

This project is intended for educational and learning purposes.

---

## Repository Maintainer

**Prasad Kusmude**

GitHub: https://github.com/prasad0443

If you find this project useful, consider giving it a star on GitHub.
