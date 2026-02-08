# AgriScale – System Architecture

AgriScale is designed as a modular AI-powered agricultural research platform.  
The system follows a layered architecture to ensure scalability, flexibility, and ease of understanding.

---

## 🏗 Architecture Overview

The platform consists of five main layers:

### 1. User Interface Layer
- Built using Lovable AI (React-based web interface)
- Allows users to interact with crop selection, soil analysis, yield prediction, and research QnA modules

---

### 2. AI Decision Engine Layer
- Crop Recommendation Engine
- Soil Analysis Engine
- Climate Suitability Engine
- Pest & Disease Analysis Engine

Each engine works independently and contributes to the final farming recommendations.

---

### 3. Machine Learning Layer
- Yield Prediction Model
- Uses input features such as crop type, soil health, climate conditions, and farming practices
- Predicts expected yield in kg/acre

---

### 4. GenAI Research Layer
- ScaleDown API integration
- Compresses long agricultural research documents by approximately 85%
- Enables fast question-answering on compressed knowledge

---

### 5. Data Layer (No Database)
- Uses CSV and JSON files for data storage
- Stores crop varieties, soil rules, and pest knowledge
- Lightweight and suitable for rapid prototyping

---

## 🔁 Data Flow

1. User inputs soil and climate details
2. Crop engine filters suitable varieties
3. Soil and climate engines analyze risks and suitability
4. ML model predicts yield
5. ScaleDown compresses research documents
6. Final precision farming report is generated

---

## 🎯 Design Goals

- No traditional database
- Fast response time
- Easy scalability
- Suitable for research and real-world extension use
