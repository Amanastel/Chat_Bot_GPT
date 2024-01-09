# Chat_Bot_GPT

## Introduction

Welcome to Chat_Bot_GPT, a Django project integrating a chatbot powered by OpenAI's GPT-3.5 Turbo. This project allows users to interact with a chatbot using the Django framework.

## Features

- **Chatbot Integration**: Utilizes OpenAI's GPT-3.5 Turbo for generating responses in the chat.
- **Real-time Interaction**: Users can engage with the chatbot in real-time, receiving responses based on their input.
- **User Authentication**: Implements user authentication for personalized chat experiences.
- **Chat History**: Stores chat interactions, providing users with a history of their conversations.

### Chat
![Home Page](https://raw.githubusercontent.com/Amanastel/Chat_Bot_GPT/main/assets/chat1.png)

### Chat
![Our Services Page](https://raw.githubusercontent.com/Amanastel/Chat_Bot_GPT/main/assets/chat2.png)

### Chat
![Upload PDF Document](https://raw.githubusercontent.com/Amanastel/Chat_Bot_GPT/main/assets/chat3.png)


## Prerequisites

Before you begin, ensure you have the following prerequisites:

- Python (3.x) installed on your system.
- Django installed (`pip install Django`).
- OpenAI API key (set it as an environment variable named `OPENAI_API_KEY`).

## Getting Started

Follow these steps to set up and run the project:

```bash
1. Clone the repository: `git clone https://github.com/Amanastel/Chat_Bot_GPT.git`
2. Navigate to the project directory: `cd Chat_Bot_GPT`
3. Create a virtual environment: `python -m venv venv`
4. Activate the virtual environment: `source venv/bin/activate` (Linux/Mac) or `venv\Scripts\activate` (Windows)
5. Apply database migrations: `python manage.py migrate`
6. Create a superuser: `python manage.py createsuperuser`
7. Run the development server: `python manage.py runserver`

## Usage

- Access the Django admin panel to manage users, chat history, and other features: [http://localhost:8000/admin/](http://localhost:8000/admin/)
- Interact with the chatbot through the application.

## API Endpoints

- **User Login:** `POST /login/`
- **User Registration:** `POST /register/`
- **User Logout:** `GET /logout/`
- **Chatbot Interaction:** `POST /chat/`

## Project Structure

```plaintext
├── chatbotapp
│   ├── migrations
│   ├── templates
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── tests.py
│   └── views.py
├── Chat_Bot_GPT
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── manage.py
└── README.md
