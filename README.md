# AI-Powered-Travel-Itinerary-Generator

A web-based travel planning application that helps users generate personalized travel itineraries based on their source, destination, travel dates, and preferences. The application combines itinerary generation, weather information, and translation features to make trip planning easier and more convenient.

## 🌍 Overview

Planning a trip can involve researching destinations, activities, weather conditions, transportation, and daily schedules. The **Travel Itinerary Generator** brings these tasks together in one application.

Users can enter their travel details and receive a structured itinerary designed around their trip duration and budget. The application also provides destination weather information and allows users to translate their itinerary into their preferred language.

## ✨ Features

* 🗺️ **Personalized Itinerary Generation**

  * Generates a day-by-day travel itinerary based on the selected source, destination, and travel dates.
  * Provides suggested activities and places to explore.

* 🌦️ **Weather Information**

  * Provides destination weather information for the selected travel period.
  * Helps users plan activities according to expected weather conditions.

* 🌐 **Itinerary Translation**

  * Allows users to translate the generated itinerary into different languages.
  * Uses the `deep-translator` library for translation.

* 👤 **User Authentication**

  * User registration and login functionality.
  * User-specific dashboard for accessing travel information.

* 💰 **Budget-Oriented Planning**

  * Generates travel suggestions while considering an optimum travel budget.

* 📱 **Responsive Web Interface**

  * Simple and user-friendly interface for planning trips.

## 🛠️ Technologies Used

### Backend

* Python
* Flask
* Flask-SQLAlchemy
* SQLAlchemy

### Frontend

* HTML
* CSS
* JavaScript
* Jinja2 Templates

### APIs & AI

* Google Generative AI / Gemini
* Visual Crossing Weather API
* Deep Translator

### Database

* SQLite

### Deployment

* Gunicorn
* WSGI



## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/Travel-Itinerary-Generator.git
cd Travel-Itinerary-Generator
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

Activate it:

**Windows**

```bash
venv\Scripts\activate
```

**macOS / Linux**

```bash
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure API Keys

Create a `.env` file in the project root:

```env
WEATHER_API_KEY=your_visual_crossing_api_key
GEMINI_API_KEY=your_gemini_api_key
```

> ⚠️ Never upload your actual API keys or `.env` file to GitHub.

### 5. Run the Application

```bash
python wsgi.py
```

The application will start locally and can be accessed through the URL shown in the terminal.

## 🔑 Required APIs

The application requires API credentials for external services used by the project:

* **Visual Crossing Weather API** – provides weather information for the destination.
* **Google Gemini API** – used for AI-powered itinerary generation.

API keys should be stored securely in environment variables.

## 🔄 Application Workflow

```text
User
  │
  ▼
Enter Travel Details
  │
  ├── Source
  ├── Destination
  ├── Travel Dates
  └── Preferences
  │
  ▼
Flask Backend
  │
  ├── AI API ──────────► Generate Itinerary
  │
  ├── Weather API ────► Destination Weather
  │
  └── Translation ────► Preferred Language
  │
  ▼
Personalized Travel Itinerary
  │
  ▼
User Dashboard
```

## 📸 Application Screenshots

### Home Page

The landing page allows users to access the travel planning application.

### User Registration & Login

Users can create an account and securely access their dashboard.

### Travel Planning

Users provide their source, destination, and travel dates to generate their trip plan.

### Generated Itinerary

The application displays a structured itinerary containing recommended activities and travel information.

## 🚀 Future Enhancements

The following features can further improve the application:

* Support for **multi-destination trips**
* Hotel and flight recommendations
* Real-time flight and hotel availability
* Google Maps integration
* Interactive destination maps
* Expense tracking and budget management
* Collaborative itinerary planning
* Save and export itineraries as PDF
* Improved personalization based on traveler interests
* Mobile-friendly Progressive Web App (PWA)

## 📌 Project Purpose

This project demonstrates the development of a travel-focused web application integrating:

* Web application development
* REST API integration
* AI-assisted content generation
* Weather data integration
* Database management
* User authentication
* Multilingual support

It can be further extended into a complete travel planning platform with real-time travel services and personalized recommendations.


### 👩‍💻 Project Note

This repository is maintained as part of my learning and practical exploration of **travel technology, web applications, API integration, and itinerary automation**.

If you find the project useful, feel free to explore the code and improve it further.
