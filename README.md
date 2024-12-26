# Resume Analyzer          
[![Live App](https://img.shields.io/badge/Live-App-brightgreen)](https://resume-analyser-kp0f.onrender.com/)




## Description

Resume Analyzer is a full-stack web application that analyzes resumes using Artificial Intelligence and provides meaningful insights such as skill extraction, resume evaluation, and improvement suggestions.

This project integrates **Google Gemini AI** for resume analysis and includes secure authentication features like email verification and password reset using **Brevo** and job suggestions using **Adzuna API**.



## Tech Stack
- Frontend: HTML, CSS, React.js  
- Backend: Spring Boot  
- Database: MySQL  



## Preview

<p align="center">
  <img width="30%" src="https://github.com/user-attachments/assets/df7bb0c1-1f10-478d-b8c9-c2b1bf2369f4" />
  <img width="30%" src="https://github.com/user-attachments/assets/1c65a0cc-c915-4103-a7fe-30a975639ab0" />
  <img width="30%" src="https://github.com/user-attachments/assets/b8ca21ad-7c2f-470d-ad5d-73119b8fd9f1" />
</p>

<p align="center">
  <img width="30%" src="https://github.com/user-attachments/assets/3f945bf1-84dd-4052-9c65-709f512ae0a4" />
  <img width="30%" src="https://github.com/user-attachments/assets/d04af8b7-4e12-4948-94c6-3b1f15340180" />
  <img width="30%" src="https://github.com/user-attachments/assets/a0c6f513-2108-41c8-98b5-91e86d27d398" />
</p>



## Frontend & Backend Integration Notes

- The frontend UI is developed using **React**
- For deployment, the React application is **built and served by the Spring Boot backend** as static files
- The React production build files are placed inside the backend’s **static** directory

### Static & Template Files
- The `static` folder contains the **React production build files**
- The `templates` folder inside `static` is used to store **email templates**
  - Used for **email verification** and **password reset**



## How to Run the Project Locally

#### 1. Clone the Repository
```bash
git clone https://github.com/Mohamed-Imran-12/Resume-Analyser.git
```

#### 2. Open Project in IDE
Open the project in **IntelliJ IDEA / Eclipse**

Open `pom.xml` and allow Maven to download dependencies

#### 3. Configure Credentials (`application.properties`)

###### Database (ONLY MySQL)
```properties
spring.datasource.url=your_DB_URL
spring.datasource.username=your_DB_USERNAME
spring.datasource.password=your_DB_PASSWORD
```

###### Google Cloud Platform (Google Sign-In)
```properties
spring.security.oauth2.client.registration.google.client-id=your_GCP_ID
spring.security.oauth2.client.registration.google.client-secret=your_GCP_SECRET
```

###### Google Gemini AI (Resume Analysis)
```properties
genKey=your_GEMINI_API_KEY
```

###### Mail Service (ONLY Brevo)
```properties
apiKey=your_BREVO_MAIL_API
```

###### Job Suggestions (ONLY Adzuna)
```properties
application-id=your_ADZUNA_APP_ID
application-api-key=your_ADZUNA_API_KEY
```

###### JWT Credentials
```properties
jwt-key=your_OWN_SECRET_KEY (Generate a secure key using any JWT secret generator)
```


#### 4. Run Backend
Run `ResumeAnalyserApplication.java`

#### 5. Open in Browser
```
http://localhost:8080/
```



## Important Notes (Must Read)

- Only **Gemini AI** is configured in this project.  
To use another AI provider, update AI-related code in `appservice.java`.

- Email functionality works **only with Brevo API**.  
To use another mail provider, update mail-related code in `mailservice.java`.

- AI models evolve quickly.  
If the configured Gemini model is removed or replaced, update the model in `appservice.java`.



## Modifying the Frontend UI

Do **not** edit files inside the backend `static` folder directly.

### 1. Run Frontend Separately (Development Mode)
```bash
cd "frontend src"
npm install
npm run dev
```

This starts the React development server for UI changes.



### 2. Build Frontend for Backend Deployment
```bash
cd "frontend src"
npm run build
```

#### Backend Static Structure
```text
static/
├── assets/
│   ├── *.css
│   ├── *.js
├── index.html
```

Steps:
- Delete old `index.html` and files inside `assets`
- Copy new build files from `dist`
- Paste them into backend `static` directory



## Disclaimer
- This project is developed for learning and demonstration purposes
- AI analysis results may vary and should not be considered professional career advice.


<!-- auto-update 2025-06-15 01:02:11 -->

<!-- auto-update 2025-06-16 01:02:11 -->

<!-- auto-update 2025-06-17 01:02:11 -->

<!-- auto-update 2025-06-18 01:02:11 -->

<!-- auto-update 2025-06-19 01:02:11 -->

<!-- auto-update 2025-06-20 01:02:11 -->

<!-- auto-update 2025-06-21 01:02:11 -->

<!-- auto-update 2025-06-22 01:02:11 -->

<!-- auto-update 2025-06-23 01:02:11 -->

<!-- auto-update 2025-06-24 01:02:11 -->

<!-- auto-update 2025-06-25 01:02:11 -->

<!-- auto-update 2025-06-26 01:02:11 -->

<!-- auto-update 2025-06-27 01:02:11 -->

<!-- auto-update 2025-06-28 01:02:11 -->

<!-- auto-update 2025-06-29 01:02:11 -->

<!-- auto-update 2025-06-30 01:02:11 -->

<!-- auto-update 2025-07-01 01:02:11 -->

<!-- auto-update 2025-07-02 01:02:11 -->

<!-- auto-update 2025-07-03 01:02:11 -->

<!-- auto-update 2025-07-04 01:02:11 -->

<!-- auto-update 2025-07-05 01:02:11 -->

<!-- auto-update 2025-07-06 01:02:11 -->

<!-- auto-update 2025-07-07 01:02:11 -->

<!-- auto-update 2025-07-08 01:02:11 -->

<!-- auto-update 2025-07-09 01:02:11 -->

<!-- auto-update 2025-07-10 01:02:11 -->

<!-- auto-update 2025-07-11 01:02:11 -->

<!-- auto-update 2025-07-12 01:02:11 -->

<!-- auto-update 2025-07-13 01:02:11 -->

<!-- auto-update 2025-07-14 01:02:11 -->

<!-- auto-update 2025-07-15 01:02:11 -->

<!-- auto-update 2025-07-16 01:02:11 -->

<!-- auto-update 2025-07-17 01:02:11 -->

<!-- auto-update 2025-07-18 01:02:11 -->

<!-- auto-update 2025-07-19 01:02:11 -->

<!-- auto-update 2025-07-20 01:02:11 -->

<!-- auto-update 2025-07-21 01:02:11 -->

<!-- auto-update 2025-07-22 01:02:11 -->

<!-- auto-update 2025-07-23 01:02:11 -->

<!-- auto-update 2025-07-24 01:02:11 -->

<!-- auto-update 2025-07-25 01:02:11 -->

<!-- auto-update 2025-07-26 01:02:11 -->

<!-- auto-update 2025-07-27 01:02:11 -->

<!-- auto-update 2025-07-28 01:02:11 -->

<!-- auto-update 2025-07-29 01:02:11 -->

<!-- auto-update 2025-07-30 01:02:11 -->

<!-- auto-update 2025-07-31 01:02:11 -->

<!-- auto-update 2025-08-01 01:02:11 -->

<!-- auto-update 2025-08-02 01:02:11 -->

<!-- auto-update 2025-08-03 01:02:11 -->

<!-- auto-update 2025-08-04 01:02:11 -->

<!-- auto-update 2025-08-05 01:02:11 -->

<!-- auto-update 2025-08-06 01:02:11 -->

<!-- auto-update 2025-08-07 01:02:11 -->

<!-- auto-update 2025-08-08 01:02:11 -->

<!-- auto-update 2025-08-09 01:02:11 -->

<!-- auto-update 2025-08-10 01:02:11 -->

<!-- auto-update 2025-08-11 01:02:11 -->

<!-- auto-update 2025-08-12 01:02:11 -->

<!-- auto-update 2025-08-13 01:02:11 -->

<!-- auto-update 2025-11-11 10:15:45 -->

<!-- auto-update 2025-11-13 10:15:45 -->

<!-- auto-update 2025-11-15 10:15:45 -->

<!-- auto-update 2025-11-17 10:15:45 -->

<!-- auto-update 2025-11-19 10:15:45 -->

<!-- auto-update 2025-11-21 10:15:45 -->

<!-- auto-update 2025-11-23 10:15:45 -->

<!-- auto-update 2025-11-25 10:15:45 -->

<!-- auto-update 2025-11-27 10:15:45 -->

<!-- auto-update 2025-11-29 10:15:45 -->

<!-- auto-update 2025-12-01 10:15:45 -->

<!-- auto-update 2025-12-03 10:15:45 -->

<!-- auto-update 2025-12-05 10:15:45 -->

<!-- auto-update 2025-12-07 10:15:45 -->

<!-- auto-update 2025-12-09 10:15:45 -->
