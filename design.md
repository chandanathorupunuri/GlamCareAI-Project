# System Design Document – GlamCareAI

## 1. System Overview

GlamCareAI is an AI-powered skincare analysis and recommendation platform. 
The system analyzes facial images using computer vision and machine learning models to provide personalized skincare recommendations.

---

## 2. System Architecture

The system follows a 3-Layer Architecture:

1. Presentation Layer (Frontend)
2. Application Layer (Backend + AI Processing)
3. Data Layer (Database + Storage)

Users upload an image → AI model processes image → Skin conditions detected → Personalized recommendations generated.

---

## 3. Technology Stack

Frontend:
- HTML
- CSS
- JavaScript

Backend:
- Node.js / Express.js

AI & ML:
- Python
- OpenCV
- TensorFlow / CNN Model

Database:
- MongoDB / Firebase

Cloud Storage:
- Image storage for uploaded photos

---

## 4. Module Design

### 4.1 User Authentication Module
- User Registration
- Login System
- Secure password encryption

### 4.2 Image Upload Module
- Camera access / Image upload
- Image preprocessing
- Secure image handling

### 4.3 AI Skin Analysis Module
- Acne detection
- Pigmentation detection
- Wrinkle detection
- Skin type classification

### 4.4 Recommendation Engine
- Personalized skincare suggestions
- Product recommendations
- Routine suggestions (morning / night)

### 4.5 Dashboard Module
- User skin history tracking
- Progress comparison
- AI insights

---

## 5. Database Design

### Users Collection
- userId
- name
- email
- password (encrypted)
- age
- skinType

### Analysis Reports Collection
- reportId
- userId
- imageURL
- detectedIssues
- recommendations
- createdAt

---

## 6. Workflow

1. User registers or logs in
2. Uploads facial image
3. Image processed by AI model
4. Skin issues detected
5. Personalized recommendations generated
6. Report stored in database
7. User views dashboard

---

## 7. Security Design

- Encrypted passwords
- Secure image storage
- Data privacy protection
- Role-based access control

---

## 8. Future Enhancements

- AI chat assistant for skincare advice
- Dermatologist consultation integration
- Mobile application
- Real-time skin improvement tracking
