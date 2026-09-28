# 🌱 CloudRoot

CloudRoot is a cloud-based IoT and AI application designed to help users monitor and manage basil plants.

The system combines real-time sensor monitoring, AI-based plant image analysis, academic information retrieval using RAG, and cloud-based data storage in a single user-friendly interface.

## ✨ Features

- 📊 **Dashboard** – Overview of plant health and sensor measurements.
- 🌡️ **Live Telemetry** – Monitor temperature, humidity, and soil moisture data.
- 📷 **Plant Scanner** – Upload basil plant images and analyze their health using an AI image classification model.
- 🔎 **Academic Search** – Search academic articles and receive answers using a Retrieval-Augmented Generation (RAG) system.
- ✅ **Task Management** – Create and manage plant-care tasks.
- 🎮 **Gamification** – Encourages consistent plant care through tasks and progress tracking.
- ☁️ **Cloud Integration** – Sensor and application data are stored and accessed through cloud services.

## 🏗️ System Architecture

CloudRoot is designed using separated services for the main system responsibilities:

### EcologicalRAG Service
Retrieves relevant academic articles and provides context to an external LLM to generate source-based answers.

A local fallback mechanism is used when the external AI service is unavailable.

### Plant Image Classifier
Uses a Hugging Face image classification model to analyze uploaded basil images and classify the plant's health status.

### Sensor Data Service
A cloud-hosted API provides access to IoT sensor measurements such as:

- Temperature
- Humidity
- Soil moisture

The frontend communicates with the sensor service through HTTP APIs.

## 🛠️ Technologies

- Python
- Gradio
- Firebase
- REST APIs
- IoT
- RAG
- Gemini API
- Hugging Face
- Machine Learning
- Render

## 🔄 Application Flow

User
↓
Gradio Interface
↓
Application Services

├── Sensor Data Service  
├── Plant Image Classifier  
├── Academic RAG Service  
└── Firebase Database

## 🎯 Project Goal

The goal of CloudRoot is to reduce uncertainty in plant care by combining IoT sensor information and AI technologies.

Instead of relying only on visual inspection, users can monitor environmental conditions, analyze plant images, search scientific information, and track plant-care activities from one system.

## 👩‍💻 My Contribution

My main responsibilities in the project included:

- Developing frontend components using Gradio.
- Connecting the user interface to the system logic.
- Integrating Firebase with the application.
- Implementing persistent storage for sensor and task data.
- Connecting UI workflows with cloud services.
- Testing the data flow between the interface and the database.

## 📚 Academic Project

CloudRoot was developed as part of the Cloud Computing course at Braude College of Engineering.
