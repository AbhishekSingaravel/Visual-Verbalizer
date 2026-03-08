# 🖼️ Visual Verbalizer – Image Caption Generator

## Overview
Visual Verbalizer is an AI-powered Image Caption Generator that automatically generates meaningful textual descriptions for images. The system combines computer vision and natural language processing techniques to convert visual information into human-readable captions.

This project uses a deep learning model to analyze image features and generate context-aware descriptions, making it useful for applications such as accessibility tools, content generation, and image indexing.

---

## Features
- Upload images and generate captions automatically
- AI-powered caption generation
- Modern web interface for interaction
- Backend API for image processing and caption generation
- Secure authentication using Clerk
- Scalable client-server architecture

---

## Tech Stack

### Frontend
- **Next.js**
- **React**
- **Clerk Authentication**

### Backend
- **Python**
- **FastAPI**
- **Uvicorn**

### AI / ML
- **Deep Learning-based Image Captioning**
- **OpenAI API**
- **Computer Vision Techniques**

---

## Project Architecture

```
User Uploads Image
        │
        ▼
Frontend (Next.js / React)
        │
        ▼
Backend API (FastAPI)
        │
        ▼
AI Model / OpenAI API
        │
        ▼
Generated Caption Returned to User
```

---

# Client Setup

## Step 1: Install Dependencies
Navigate to the client directory and install dependencies:

```bash
cd client
npm install
```

---

## Step 2: Configure Environment Variables

Create a `.env` file inside the **client** directory.

Example configuration:

```
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
CLERK_SECRET_KEY=your_clerk_secret_key

NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

OPENAI_API_KEY=your_openai_api_key
```

Replace the placeholder values with your actual credentials.

---

## Step 3: Start the Client

Run the following command inside the client directory:

```bash
npm run dev
```

The client application will start locally.

---

# Server Setup

## Step 1: Create and Activate Virtual Environment

Navigate to the server directory:

```bash
cd server
```

Create a virtual environment if it doesn't exist:

```bash
python -m venv .venv
```

Activate the environment:

Windows:

```bash
.venv\Scripts\activate
```

Linux / Mac:

```bash
source .venv/bin/activate
```

---

## Step 2: Run the Backend Server

Start the FastAPI server using Uvicorn:

```bash
uvicorn api:app --reload
```

The server will run at:

```
http://localhost:8000
```

---

# Running the Project

1. Start the backend server
2. Start the frontend client
3. Upload an image through the web interface
4. The system processes the image and generates a caption

---

# Applications
- Assistive tools for visually impaired users
- Automatic image description generation
- Content creation platforms
- Image indexing and search systems

---

# Future Improvements
- Improve caption accuracy using larger training datasets
- Integrate transformer-based vision-language models
- Add multilingual caption support
- Deploy as a cloud-based AI service

---

# Author

**Abhishek Singaravel**  
Backend Developer | AI Enthusiast

LinkedIn:  
https://linkedin.com/in/abhishek-singaravel-698b35250

GitHub:  
https://github.com/AbhishekSingaravel
