# hackathon-sample-app

## Overview
hackathon-sample-app is a simple FastAPI-based web application that serves as a starting point for hackathon projects. It provides basic endpoints for demonstration purposes and can be easily extended for more complex applications.

## Features
- Hello World endpoint
- Item retrieval endpoint with optional query parameter

## Prerequisites
- Python 3.7 or higher
- Docker (optional, for containerized deployment)

## Installation

### Local Installation
1. Clone the repository:
   ```
   git clone https://github.com/martilar/hackathon-sample-app.git
   cd hackathon-sample-app
   ```

2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

3. Run the application:
   ```
   python app.py
   ```

### Docker Installation
1. Build the Docker image:
   ```
   docker build -t hackathon-sample-app .
   ```

2. Run the container:
   ```
   docker run -p 8000:8000 hackathon-sample-app
   ```

## Usage

Once the application is running, you can access the following endpoints:

1. Root endpoint:
   ```
   GET /
   ```
   Returns a "Hello World" message.

2. Items endpoint:
   ```
   GET /items/{item_id}
   ```
   Retrieves an item by its ID. You can also include an optional query parameter `q`.

   Example: `GET /items/5?q=search_query`

## Project Structure
```
.
├── .github
│   └── workflows
│       └── main.yml
├── Dockerfile
├── README.md
├── app.py
├── compose.yaml
├── credential.json
└── requirements.txt
```

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## License
[Include your license information here]
