# App Development Deliverables

## 1. Executable Code

- The application code is structured to be executed without major setup issues.
- The codebase is managed using Git for version control, ensuring a clear and organized commit history that tracks development progress and changes.

## 2. Documentation

### a. Inline Code Comments

- The code includes detailed inline comments to enhance readability and provide clarity on logic implementation.

### b. Comprehensive Report

#### Solution Architecture

- The application consists of a web interface that allows users to submit **Shopify product URLs** and images for advertisement purposes.
- The **frontend** is built using **React (TypeScript)** and **Material UI** to provide a modern, user-friendly interface.
- The **backend** is powered by **FastAPI**, handling authentication, product processing, and API integration.
- The system supports extracting **product details from Shopify JSON API** and enables ad campaign creation for platforms like Meta and Google Ads.
- The backend stores **product details** in a structured format and supports **session-based authentication.**

#### Design Choices and Technology Stack Rationale

- **Backend:** Python with FastAPI for efficient API handling and scalability.
- **Frontend:** React.js with TypeScript for a responsive and maintainable UI.
- **Database:** In-Memory for now (Can be migrated to SQL/NoSQL DB in future)

#### Setup, Run, and Test Instructions

### Setup

- Setup Instructions are provide in the respective repos of front-end and back-end.

### Run

- Start the backend server:
  ```bash
  uvicorn main:app --host 0.0.0.0 --port 8000 --reload
  ```
- Start the frontend:
  ```bash
  npm start
  ```

### Test

- API tests using Postman.

#### Assumptions and Limitations

- **Assumptions:**
  - Users provide valid Shopify product links.
  - API keys and authentication credentials are available for external services.
  - The ad platform APIs used for launching creatives are accessible.
- **Limitations:**
  - May not support all Shopify store themes or custom modifications.
  - Performance constraints based on Shopify and third-party API rate limits.

## 3. API and Tool Usage

- **APIs Used:**
  - **Shopify API** for extracting product details(https://birdrockbaby.com/).
  - **Firebase Authetication** for Authetication.
  - **Ad platform API** (Meta/Google Ads) for launching creatives.

## 4. Features Overview

- ✅ **Secure User Authentication & Session Management**
- ✅ **Product Scraping from Shopify JSON API**
- ✅ **FastAPI-powered Backend with API Documentation** (`/docs` endpoint)
- ✅ **Modern, Responsive UI with Material UI & React**

---

This README file serves as a structured guideline covering all essential deliverables required for the application development.

