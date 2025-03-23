# Gridworld Environment and Value Iteration

This is a Flask-based grid map application that implements the policy evaluation algorithm in reinforcement learning.

![image](https://github.com/user-attachments/assets/faaf425c-d2db-443e-b378-dcbf7e34c818)


## Features

- Generate a customizable grid (from 3x3 to 10x10)  
- Set a start point (green) and an endpoint (red)  
- Add obstacles (gray)  
- Generate a random policy  
- Compute and display the value of each cell  

## Running with Docker

### Using Docker Compose (Recommended)

1. Ensure Docker and Docker Compose are installed.  
2. Run the following command in the project root directory:

    ```bash
    cd grid_app
    docker-compose up -d
    ```

3. Visit `http://localhost:5000`

## Running Locally (Without Docker)

1. Install dependencies:

    ```bash
    pip install -r requirements.txt
    ```

2. Run the application:

    ```bash
    python app.py
    ```

3. Visit `http://localhost:5000`
