# 🏆 Social Influencer Platform & Lifestyle Competition


Rebuilding from the foundation of the 2022 social influencer platform, this project evolves into a modern competition system and lifestyle platform. A digital ecosystem where influencers and creators can host, join, and promote healthy lifestyle challenges and services.


## 📖 Overview

**Social Influencer Platform** is a next-generation **AI-powered social competition platform** designed to automatically score and rank participants using intelligent agent systems.  

It integrates modern **AI frameworks**, **Node.js**, **Angular**, and **Azure services** to create an interactive, scalable, and secure digital competition environment.

Originally started as a prototype system "PTPro - Social platform" etablished in around **2017**, the project is able to be reimagined and rebuilt using today’s powerful AI and cloud technologies.  

This README describes the **background**, **architecture**, **stack**, **features**, **installation**, and **key learnings** from the project.

---

## 🧭 Background

### Original Vision (2017)
The Social Influencer Platform is a next-generation social and lifestyle engagement system that allows influencers and users to participate in lifestyle competitions.
It provides a space where participants can:

### Early Success
- Review **Social influencer platform** have recieved good feedbacks regarding the need of a compition based social platform. 
- Join or host public and private challenges or sales.
- Showcase and sell their lifestyle or wellness services.
- Track rankings, engagement, and progress in real time.

### The history
The project was discontinued in 2022 due to:
- API dependencies on discontinued social media services.
- Limited AI technology for complex performance and gesture recognition.
- Infrastructure and scaling challenges for live competitions.

---

## 🤖 Overview

With the advancements in modern AI and cloud technology, the project has been **revived** and redesigned as new complete **Social Influencer Platform system**.

The version leverages:
- **Node.js and Angular** for full-stack, modular web development.
- **Docker** for containerized deployments and developer sandboxing.
- **Microsoft Agent Framework** for orchestrating intelligent decision-making.


---

## 🏗️ Architecture Overview

The **Compition** system is designed with a **modular monorepo architecture** to ensure scalability, maintainability, and team collaboration.

### 🔹 High-Level Structure
```bash
/virtual-contest
│
├── /server # Backend (Node.js API)
│ ├── /models # Sample data models (dummy data)
│ ├── /routes # API routes (authentication, scores, users)
│ ├── /middleware # JWT authentication & security layers
│ ├── /controllers # API logic and handlers
│ └── server.js # Application entry point
│
├── /client # Angular Frontend
│ ├── /src/app/modules # Feature modules (leaderboard, profile, judge)
│ ├── /src/environments # Environment configs
│ ├── angular.json # Angular configuration file
│ └── package.json # Frontend dependencies
│
├── /config # Global configs and environment setup
├── /docker # Dockerfile and docker-compose setup
├── .env.example # Example environment configuration
└── README.md # Documentation
```

### 🔹 Data Flow Diagram

1. User submits performance data (api/data/metrics).
2. Backend receives the submission through the API.
3. Operator-agent processes the submission using:
   - Models for resource recognition.
   - Azure Cloud for verification.
4. Scoring and ranking logic updates the database (PostgreSQL).
5. Leaderboards update in real-time on the Angular frontend.

---

## 🧠 Technology Stack Overview (Upgradable)

| Category | Technology | Purpose |
|-----------|-------------|----------|
| **Frontend** | Angular | User interface and leaderboard visualization |
| **Backend** | Node.js (Express) | API server, business logic, and JWT authentication |
| **Machine Learning** | GPT-4, TensorFlow | AI-driven data processing |
| **Database** | PostgreSQL (vector extensions) | Stores competition data and vector embeddings |
| **Cloud** | Azure Web Services | Hosting, scalability, and AI model integration |
| **Resource handling** | Azure Computer | Participant submission analysis |
| **Authentication** | JWT (JSON Web Token) | Secure login and data access |
| **Containerization** | Docker | Developer isolation and environment consistency |
| **Version Control** | Git (Private Repository) | Code management and team collaboration |

## 📈 Future Roadmap

- 💬 Add social chat and group collaboration tools.
- 🛒 Integrate payments for influencer services.
- 📱 Launch a mobile-friendly Progressive Web App (PWA).
- 🧾 Enable analytics dashboards for influencer engagement tracking.
- 🌍 Support multi-language localization.

## 🌟 Key Features

### ⚙️ Core Functionalities
- **AI Judging System** – Automated evaluation using vision and data models.  
- **Dynamic Leaderboards** – Real-time ranking of participants.  
- **JWT Authentication** – Secure login and data handling.  
- **Data Models** – For demo and testing without sensitive information.  
- **Azure Integration** – Cloud-based AI and data storage.  
- **Modular Codebase** – Backend and frontend separated into submodules.  
- **Dockerized Environment** – Fast setup and deployment.  

### 🔒 Security Features
- Role-based developer access.
- Secrets managed via `.env` files and Azure Key Vault.
- Enforced HTTPS and CORS for API requests.
- Authentication tokens used across frontend and backend services.

### 🧪 Testing & Quality
- Unit testing for API functions.
- Integration testing for API endpoints and frontend communication.
- Plan for future E2E (end-to-end) testing using Cypress or Playwright.

---

## ⚙️ Installation & Setup

### 🔧 Prerequisites
Before running the project, ensure you have:
- Node.js (v18 or later)
- Angular CLI
- Docker & Docker Compose
- PostgreSQL (if not using Docker)
- Azure credentials (optional, for AI integration)

---

### 🖥️ Installation Steps

1. **Clone the Repository**
```bash
git clone https://github.com/Public-Research-Foundation/Social-Competition-Platform
cd Social-Competition-Platform
```

2. **Install Backend Dependencies**
```bash
cd server
npm install
 ```

3. **Install Frontend Dependencies**
```bash
cd ../client
npm install
```

4. **Set Up Environment Variables**
```bash
DB_URL=postgres://user:password@localhost:5432/virtualcontest
JWT_SECRET=your_jwt_secret
AZURE_KEY=your_azure_key
```

5. **Run with Docker (Recommended)**
```bash
docker-compose up --build
```

6. **Access the Application**
```bash
Frontend: http://localhost:4200
Backend API: http://localhost:3000/api
```

## 🧩 Module Breakdown

| Module | Description |
|--------|--------------|
| **Auth Module** | Handles user login, registration, and JWT validation. |
| **Operator Module** | AI agent for analyzing sports submissions and generating scores. |
| **Leaderboard Module** | Displays real-time rankings, points, and competition progress. |
| **Admin Module** | Provides an admin dashboard for managing competitions, users, and results. |
| **User Module** | Manages athlete profiles, participation records, and competition history. |

Each module is developed as a **self-contained unit** to improve scalability, maintainability, and collaboration across the development team.

---

## ☁️ Cloud Integration (Azure)

The platform is deeply integrated with **Azure Web Services** to ensure scalability, performance, and AI functionality.

| Azure Service | Role |
|----------------|------|
| **Azure Computer Vision** | Processes and analyzes resource submissions for competition. |
| **Azure Web Apps** | Hosts the backend and frontend services. |
| **Azure Key Vault** | Securely manages API keys, environment variables, and credentials. |
| **Azure PostgreSQL** | Provides a managed relational database for competition data. |
| **Azure Agent Framework** | Enables AI agent orchestration and automated decision-making. |

---

## 🔐 Developer Access & Security Strategy

The original project was maintained as a **private repository** with **invitation-only access** and **role-based permissions** for developers.

### 🛡️ Security Best Practices Implemented
- 🚫 No direct exposure of secrets or credentials.  
- 🔑 Protected API endpoints using **JWT authentication**.  
- 🐳 Utilized **Docker environments** for safe, isolated local development.  
- 👥 Enforced **role-based controls** for both repository and production access.  

> 💡 **Tip:** For enhanced isolation, use **sandboxed Docker environments** or **container-based CI/CD runners** to prevent unauthorized file access and improve security compliance.

---

## 🧱 Project Highlights

- ⚙️ **Modular full-stack architecture** built with Node.js and Angular.  
- 🤖 **Compute integration** through Azure and custom judging agents.  
- 🐳 **Containerized deployment** via Docker for consistent environments.  
- 🧩 **Data and sample models** for safe and efficient testing.  
- 🔒 **JWT-secured authentication** ensuring data integrity and privacy.  
- ☁️ **Cloud-ready infrastructure** designed for scalability and integration.  
- 🔁 **CI/CD-ready pipelines** for automated testing and continuous deployment.  

---

## 📈 Future Roadmap

- 🧠 Integrate **advanced GPT-based logic** for more nuanced evaluation.  
- 🔒 Migrate to **zero-trust, containerized environments** for enhanced isolation.  
- ⚙️ Add **continuous integration and testing pipelines** using GitHub Actions.  
- 📊 Develop **public APIs** for third-party sports competition management systems.  
- 🌐 Release an **open-source starter kit** for social competition platforms.  

---

## 🏁 Conclusion

The **Social Influencer Platform** project illustrates how **modern frameworks, and cloud computing** can transform sports competitions.  
By combining **automation**, **fairness**, and **scalability**, this platform provides a practical blueprint for future **AI-driven social systems**.

This repository highlights both the **technical depth** and **architectural foresight** behind the project — evolving from a private licensed framework into a **modern, modular, and public-ready social platform**.

---

## ⚖️ License

**This project was originally developed using extension with **private licensed template** and therefore does **not** include any proprietary or commercial assets from the original system.**

The current version of **system** has been fully restructured using **publicly shareable code**, **mock data**, and **open integrations** suitable for demonstration and educational purposes.


### 📝 Recommended License: MIT License

The **MIT License** is an excellent fit for this project because it:
- ✅ Allows others to **use, modify, and distribute** the code freely.  
- ✅ Requires that attribution to the original author be maintained.  
- ✅ Is **business-friendly**, meaning it can be used for both open-source and commercial purposes.  
- ✅ Keeps the licensing simple while protecting your ownership rights.

You can include the following license file in your repository:

### 📄 LICENSE

MIT License

Copyright (c) [2025] [Elias Research]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

---

## 👨‍💻 Author

**[Elias Research]**  
Full-Stack Developer | AI & Cloud Engineer  
📧 [arbeidspost.efa@outlook.com]  
🌐 [[Your LinkedIn or Portfolio Link](https://www.linkedin.com/in/elias-a-8591b4173/)]