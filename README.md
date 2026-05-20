
<p align="center">
  <img src="https://img.shields.io/badge/Backend-Django%205.1.2-092E20?style=flat&logo=django&logoColor=white" />
  <img src="https://img.shields.io/badge/Engine-Django%20Templates-092E20?style=flat&logo=django&logoColor=white"/>
        <img src="https://img.shields.io/badge/UI-Bootstrap%205.3.3-7952B3?style=flat&logo=bootstrap&logoColor=white"/>
  <img src="https://img.shields.io/badge/API-OpenWeatherMap-EB6E4B?style=flat&logo=openweathermap&logoColor=white" />
  <img src="https://img.shields.io/badge/Forms-Crispy%20Forms-0769AD?style=flat&logo=django&logoColor=white" />
  <img src="https://img.shields.io/badge/Database-SQLite3-003B57?style=flat&logo=sqlite&logoColor=white" />
</p>

<h1 align="center">🌦️ Django Weather API Insight</h1>

<p align="center"><strong>A professional, responsive full-stack weather tracking workspace built with Django 5.1 and Bootstrap 5. Features real-time climate data via OpenWeather API, a custom email-based authentication architecture, and isolated user dashboards. 🚀</strong></p>

<div align="center">
  <h3>
    <a href="https://umit8108.pythonanywhere.com/">
      🖥️ Live Demo
    </a>
     | 
    <a href="https://github.com/umitarat-dev/django-weather-api-insight.git">
      📂 Repository
    </a>
  </h3>
</div>

<p align="center">
  <a href="https://umit8108.pythonanywhere.com/">
    <img src="./assets/weather-app.gif" alt="Weather App Showcase" width="700"/>
  </a>
</p>

## 📚 Navigation
- [🚀 Live Application](#-live-application)
- [👀 Application Previews](#-application-previews)
- [📦 Key Features](#-key-features)
- [🛠️ Built With](#️-built-with)
- [⚙️ Setup & Installation](#️-setup--installation)
- [📬 Contact Information](#-contact-information)

## 🚀 Live Application
The application is fully optimized, secured, and deployed in a production-ready cloud environment. Anonymous visitors are prompted to register or log in to access their isolated, personalized weather dashboard.
* **Production URL:** [https://umit8108.pythonanywhere.com/](https://umit8108.pythonanywhere.com/)


## 👀 Application Previews

### User Authentication (Custom Email Backend)
<em>Seamless registration and login flows utilizing a custom-built EmailAuthenticationForm over the default Django username architecture.</em>

### Personalized Weather Dashboard
<em>Real-time climate data fetching, displaying dynamic icons, temperatures, and detailed conditions with glassmorphism UI cards.</em>



## 📦 Key Features
* **Real-Time API Integration:** Seamlessly connects to the OpenWeatherMap API, fetching highly accurate climate data, temperature (Celsius), and weather icons, backed by robust `requests` error handling.
* **Custom Email Authentication:** Overrides default Django behaviors by implementing a secure, custom `EmailAuthenticationForm`, allowing users to log in with their email addresses (an industry-standard UX practice).
* **Smart Relational Database Design:** Employs a Many-to-Many (`ManyToManyField`) architectural relationship for cities. This prevents database bloating by linking a single city record to multiple users rather than creating duplicate entries.
* **Modern UI & Glassmorphism:** Front-end layout rendered using `django-crispy-forms` customized for Bootstrap 5.3. Features a dynamic smart-navbar with intelligent hover-states, floating cards with hover-elevation, and a responsive CSS structure.
* **Environment Configuration:** Leverages `python-decouple` to ensure absolute security for sensitive credentials (`SECRET_KEY`, `API_KEY`, `CSRF_TRUSTED_ORIGINS`) across both local and production environments.



## 🛠️ Built With
* **Core Framework:** [Django 5.1.2](https://www.djangoproject.com/) (Python MVT Architecture)
* **Language Environment:** Python 3.11+
* **External API:** [OpenWeatherMap API](https://openweathermap.org/api)
* **Form Layout Engine:** [django-crispy-forms](https://django-crispy-forms.readthedocs.io/) & Crispy-Bootstrap5
* **Frontend UI Components:** Bootstrap 5.3.3, Custom CSS3 Utilities


## ⚙️ Setup & Installation

### 1. Clone the Repository
```bash
git clone https://github.com/umitarat-dev/django-weather-api-insight.git
cd django-weather-api-insight
```

### 2. Virtual Environment Preparation (Cross-Platform)
Instantiate a clean virtual environment utilizing Python 3.11:

macOS / Linux:
```bash
python3.11 -m venv env
source env/bin/activate
```

Windows:
macOS / Linux:
```bash
python3.11 -m venv env
source env/bin/activate
```

### 3. Install Dependencies
```bash
pip install --upgrade pip
pip install -r requirements.txt
```

### 4. Environment Variables Configuration
Create a .env file directly in the root directory (at the same level as manage.py) and populate it with the following blueprint. You will need to obtain a free API key from OpenWeatherMap:

```bash
SECRET_KEY=your_secure_local_django_secret_key
DEBUG=True
ALLOWED_HOSTS=127.0.0.1,localhost
CSRF_TRUSTED_ORIGINS=[http://127.0.0.1:8000](http://127.0.0.1:8000),http://localhost:8000

# OpenWeather API Configuration
API_KEY=your_openweathermap_api_key_here
```


### 5. Database Migrations & Server Activation
```bash
# Apply migrations
python manage.py makemigrations
python manage.py migrate

# Run the application
python manage.py runserver
```
Navigate to http://127.0.0.1:8000/ in your browser to explore the platform.



## 📬 Contact Information

I am actively open to corporate discussions regarding production backend architecture, software lifecycle deployments, and full-stack engineering vacancies.

* **LinkedIn:** [linkedin.com/in/umit-arat](https://www.linkedin.com/in/umit-arat/)
* **Email:** [umitarat8098@gmail.com](mailto:umitarat8098@gmail.com)
* **GitHub:** [github.com/umitarat-dev](https://github.com/umitarat-dev) (Current Workspace)