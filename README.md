# CitizenAI: Smart City Analysis & Civic Engagement Assistant

## 1. Introduction
**Project Title:** CitizenAI – Smart City Analysis & Civic Engagement Assistant  

**Team Members:**
1. SUBASRI.V  
2. SAHEENA BANU.S  
3. SAFIKA BANU.A.H  
4. SANDHIYA.G.S  

---

## 2. Project Overview

### Purpose
CitizenAI is an **AI-powered platform** designed to enhance urban governance, public awareness, and citizen engagement by leveraging **natural language processing (NLP)**.  

It integrates a **state-of-the-art language model** with a user-friendly interface to provide meaningful insights into **urban safety, infrastructure, and government services**.  

At its core, CitizenAI serves two primary functions:
1. **City Analysis Module** – Users enter a city name to get a detailed safety overview (crime index, accident statistics, traffic safety data, etc.).  
2. **Citizen Services Module** – Virtual civic assistant answering queries on government policies, public services, and community issues.  

This ensures citizens can access **accurate, context-aware information**, fostering **trust and transparency** between people and governing institutions.  

### Features
#### City Analysis
- Accepts the name of any city as input.  
- Generates a **crime index overview**.  
- Provides **accident and traffic safety statistics**.  
- Summarizes **overall city safety**.  
- Identifies **urban risks and challenges**.  

#### Citizen Query Handling
- Accepts **open-ended queries**.  
- Provides info on **public services** (transport, healthcare, education, etc.).  
- Explains **government policies and civic rules**.  
- Addresses **community-related issues**.  

#### AI-Powered Language Generation
- Uses **IBM Granite (transformer-based LLM)**.  
- Generates **human-like, coherent, and context-aware** responses.  
- Adapts answers to user input.  
- Removes prompt repetition for clean outputs.  

#### Interactive User Interface
- Built with **Gradio Blocks**.  
- Two main tabs: **City Analysis** & **Citizen Services**.  
- Input/output via textboxes.  
- Buttons: **Analyze City** & **Get Information**.  

#### Automation & Efficiency
- Processes inputs automatically.  
- Provides **instant, real-time reports**.  
- Saves time compared to traditional research.  

#### Scalability & Flexibility
- Works with multiple **cities and civic topics**.  
- Easily **scalable with external datasets/models**.  

#### Accessible Deployment
- Runs on **Google Colab** with minimal setup.  
- Provides **shareable public link**.  
- Supports **CPU/GPU environments**.  

---

## 3. Architecture

### I. Frontend (Gradio)
- Simple, web-based UI.  
- Tabs: **City Analysis** & **Citizen Services**.  
- Input/output handled via textboxes.  
- Buttons trigger backend functions.  

### II. Backend (Google Colab + Hugging Face)
- Colab executes logic and dependencies.  
- Uses `torch`, `transformers`, `gradio`, `accelerate`.  
- Optional **GPU acceleration**.  

### III. LLM Integration (Granite LLM via Hugging Face)
- Core: **IBM Granite 3.2-2B-Instruct** model.  
- Hugging Face `AutoTokenizer` & `AutoModelForCausalLM`.  
- Parameters: `max_length`, `temperature`, `do_sample`.  

### IV. Data Handling & Analytics
- Tokenizes, processes, and structures user inputs.  
- City module: crime index, accidents, safety.  
- Citizen module: civic policies & services.  
- Outputs cleaned and formatted.  

### V. Deployment
- Current: **Google Colab** (demo).  
- Future: **Hugging Face Spaces** for scalable hosting.  
- Runs on **CPU/GPU**.  

---

## 4. Setup Instructions

### Prerequisites
- Google account (for Colab).  
- Hugging Face account.  
- Internet connection.  

### Installation
1. Open **Google Colab**.  
2. Install required libraries:  
   ```bash
   pip install gradio
   pip install transformers
   pip install torch
