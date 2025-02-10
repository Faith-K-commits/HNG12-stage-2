# FastAPI Book Management System

This project is a simple book management system built with FastAPI. It allows you to create, read, update, and delete books from an in-memory database. The project also includes a health check endpoint and is configured for deployment on DigitalOcean with Nginx.

## Features

- **Create a Book**: Add a new book to the database.
- **Retrieve Books**: Get a list of all books or a specific book by ID.
- **Update a Book**: Update the details of an existing book.
- **Delete a Book**: Remove a book from the database.
- **Health Check**: Check if the server is active.

## Installation

1. **Clone the repository**:
   ```bash
   git clone git@github.com:Faith-K-commits/HNG12-stage-2.git
   cd HNG12-stage-2
   ```

2. **Create and activate a virtual environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate
   ```

3. **Install the dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

## Running the Application

1. **Start the FastAPI server**:
   ```bash
   uvicorn main:app 
   ```

2. **Access the API documentation**:
   Open your browser and navigate to `http://127.0.0.1:8000/docs` to view the interactive API documentation.

## Running Tests

1. **Install `pytest`** (if not already installed):
   ```bash
   pip install pytest
   ```

2. **Run the tests**:
   ```bash
   pytest
   ```

## Deployment

The project is configured for deployment on DigitalOcean with Nginx. The deployment process is automated using GitHub Actions.

1. **Set up your DigitalOcean server** and ensure you have the necessary SSH access.

2. **Configure GitHub Secrets** with your DigitalOcean server details:
   - `DROPLET_IP`
   - `DROPLET_USER`
   - `DROPLET_SSH_KEY`

3. **Push to the `main` branch** to trigger the deployment workflow.