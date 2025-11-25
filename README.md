# Medical Consultation System

![Django](https://img.shields.io/badge/Django-4.2.3-092E20?style=for-the-badge&logo=django&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.11-3776AB?style=for-the-badge&logo=python&logoColor=white)

## Overview

A comprehensive web application designed to streamline the management of medical consultations. This system facilitates the interaction between patients and doctors, handling scheduling, availability management, and specific medical service tracking.

**Purpose**: This system was developed for public dental hospitals at the Federal University of Alagoas (UFAL - Universidade Federal de Alagoas), providing an efficient solution for managing dental consultations and appointments.

## Key Features

- **Patient Management**: User registration, profile management, and history tracking.
- **Doctor Administration**: 
  - Manage profiles with specific medical specialties (e.g., Aftas, Hypersensitivity, Neuralgia).
  - Configurable weekly work schedules (Mon-Sat).
- **Smart Scheduling**: 
  - Appointment booking validation against doctor availability.
  - Support for multiple service types (Consultation, Post-surgery, Lesions, etc.).
  - Holiday awareness using the `holidays` library.
- **Admin Dashboard**: Full control over system entities via the Django Admin interface.

## Tech Stack

- **Core**: Python 3.11
- **Framework**: Django 4.2.3
- **Database**: SQLite (default) / PostgreSQL (supported via `psycopg`)
- **Frontend**: Bootstrap 4, jQuery, HTML5/CSS3

## 🚀 Getting Started

### Prerequisites

- Python 3.11+
- `pip` (Python Package Manager)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/consultas-system.git
   cd Consultas
   ```

2. **Set up a Virtual Environment**
   ```bash
   # Linux/macOS
   python3 -m venv venv
   source venv/bin/activate

   # Windows
   python -m venv venv
   venv\Scripts\activate
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Database Migration**
   Initialize the database schema:
   ```bash
   python manage.py migrate
   ```

5. **Create Superuser (Optional)**
   For admin access:
   ```bash
   python manage.py createsuperuser
   ```

6. **Run the Development Server**
   ```bash
   python manage.py runserver
   ```
   The application will be available at [http://127.0.0.1:8000/](http://127.0.0.1:8000/).

## 📂 Project Structure

- `consultas/`: Handles appointment logic and service types.
- `medico/`: Manages doctor profiles, specialties, and schedules.
- `paciente/`: Handles patient registration and data.
- `datas/`: Utilities for date and availability management.
- `pages/`: Static pages (About, Home).
- `sistema_de_consultas/`: Main project configuration.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License.

