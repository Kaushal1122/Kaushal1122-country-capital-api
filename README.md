# Country Capital API

## Overview

Country Capital API is a Python-based API that returns the country
corresponding to a given capital city.

The API is built using Flask and served using the Uvicorn ASGI server.

## Prerequisites

Before setting up the project locally, make sure you have:

- Python installed
- pip installed
- Git installed

## Local Setup

### 1. Clone the repository

git clone <repository-url>

### 2. Navigate to the project directory

cd country-capital-api

### 3. Create a virtual environment

python -m venv venv

### 4. Activate the virtual environment

#### Windows

venv\Scripts\activate

#### Linux/macOS

source venv/bin/activate

### 5. Install dependencies

pip install -r requirements.txt

## Running the API

Start the API using Uvicorn.

<appropriate uvicorn command>

The API will then be available locally.

## API Usage

The API accepts a capital city and returns the corresponding country.

The organization also provides the following microservice endpoint:

https://example.com/country-capital/<query-params>

This endpoint can be consumed by other projects within the organization.
