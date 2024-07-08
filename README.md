# Django Render Demo

This is a simple Django project demonstrating how to create a basic web application that can be deployed on Render. It includes a simple "Hello, World!" view and configuration for deployment.

## Project Structure

django_render_demo/
│
├── hello/                 # Django app
│   ├── migrations/
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── tests.py
│   └── views.py
│
├── mysite/                # Django project
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
├── .gitignore
├── build.sh
├── manage.py
├── README.md
├── render.yaml
└── requirements.txt

## Features

- Simple "Hello, World!" application
- Ready for deployment on Render

## Prerequisites

- Python 3.8 or higher
- pip
- virtualenv (recommended)

## Local Development Setup

1. Clone the repository:
   git clone https://github.com/sajan69/django_render_demo.git
   cd django_render_demo

2. Create and activate a virtual environment:
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

3. Install the required packages:
   pip install -r requirements.txt

4. Run migrations:
   python manage.py migrate

5. Start the development server:
   python manage.py runserver

6. Open your browser and navigate to `http://localhost:8000` or click on link that is provided in the terminal to see the application running.

## Deployment on Render

This project is configured for easy deployment on Render. Here's how to deploy it:

1. Create a new Web Service on Render and select your GitHub repository.
2. Render will automatically detect the `render.yaml` file and configure your service.
3. Click "Create Web Service" to deploy your application.

## Configuration Files

- `render.yaml`: Contains the configuration for Render deployment.
- `build.sh`: Script that Render uses to build and set up your application.
- `requirements.txt`: Lists all Python dependencies for the project.

## Contributing

Feel free to fork this project and submit pull requests with any improvements or suggestions.

## License

This project is open-source and available under the MIT License.