[![CI](https://github.com/mozaloom/Python-MLOps-Cookbook/actions/workflows/main.yml/badge.svg)](https://github.com/mozaloom/Python-MLOps-Cookbook/actions/workflows/main.yml)
# ML Deployment Toolkit

A containerized ML application ready for multi-cloud deployment on AWS, GCP, and Azure.

## Overview

ML Deployment Toolkit provides a production-ready machine learning application with built-in deployment patterns for various cloud environments. This repository showcases a Flask-based prediction API that can be easily deployed to multiple target environments through containerization.

## Features

- **Containerized Application**: Packaged with Docker for consistent deployment
- **ML Prediction Service**: Baseball statistics prediction model included as an example
- **Multi-Cloud Ready**: Deployment recipes for AWS, GCP, and Azure
- **AWS Lambda Integration**: Serverless deployment option using AWS SAM
- **CLI Tools**: Command-line utilities for model operations and maintenance
- **Testing Framework**: Unit tests for model library functions

## Getting Started

### Prerequisites

- Python 3.7+
- Docker
- Make (for using the Makefile commands)

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/ml-deployment-toolkit.git
cd ml-deployment-toolkit

# Set up virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### Running Locally

```bash
# Run Flask application directly
python app.py

# Or use Docker
./run_docker.sh
```

### Making Predictions

```bash
# Use the prediction script
./predict.sh
```

## Deployment Options

The repository includes various deployment recipes:

- **AWS Lambda**: Serverless deployment using AWS SAM (see `recipes/aws-lambda-sam`)
- **Docker Container**: General-purpose containerized deployment
- Additional cloud targets can be implemented using the provided patterns

## Project Structure

```
.
├── app.py                  # Main Flask application
├── cli.py                  # Command line interface
├── mlib.py                 # Model library functions
├── model.joblib            # Pre-trained model
├── Dockerfile              # Container definition
├── Makefile                # Build automation
├── recipes/                # Deployment recipes for different platforms
│   └── aws-lambda-sam/     # AWS Lambda deployment with SAM
└── utils/                  # Utility scripts
```

## License

This project is licensed under the terms included in the LICENSE file.

## Contributing

Contributions to add new deployment targets or improve existing functionality are welcome!
