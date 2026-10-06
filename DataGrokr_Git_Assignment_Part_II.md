## Part 1 – Writing a Good README

### Country Capital API

#### What is this project?

`country-capital-api` is a Python-based API that returns the name of a country when a capital city is provided.

The API is built using Flask and is served using the Uvicorn ASGI server.

#### Prerequisites

The following are required to set up and run the project locally:

- Python
- pip
- Git

#### Local Development Setup

1. Clone the `country-capital-api` repository.

2. Navigate to the project directory:

```bash
cd country-capital-api
```

3. Create and activate a Python virtual environment.

4. Install the required project dependencies.

5. Start the API using the Uvicorn server.

The API can then be accessed from the local development environment.

#### API Endpoint

A microservice endpoint is also available for other projects within the organization to consume the API:

```text
https://example.com/country-capital/<query-params>
```

The endpoint accepts a capital city as a query parameter and returns the corresponding country.

---

## Part 2 – Using .gitignore

### .gitignore

The following `.gitignore` rules are used to prevent the specified repository artifacts from being tracked:

```gitignore
/build/
*.env
/test-runs/logs
*.csv
```

### Rules Explained

- `/build/` – Ignores all files inside the `build` directory at the root of the repository.
- `*.env` – Ignores all files ending with `.env`.
- `/test-runs/logs` – Ignores all files inside the `test-runs/logs` directory.
- `*.csv` – Ignores all CSV files anywhere in the repository.

---

## Part 3 – Raising a Clean Pull Request

### PR Title

```text
feat/FEAPP-420: Allow customer notification via WhatsApp
```

### PR Description

**WHAT:**

Added support for customers to provide their WhatsApp number as an optional notification channel. When a WhatsApp number is specified, product update notifications will be sent to both the customer's email address and WhatsApp number. Customers who do not provide a WhatsApp number will continue to receive notifications through email.

**WHY:**

Customers have requested the ability to receive product update notifications through WhatsApp in addition to email. This change provides an additional notification option while keeping WhatsApp notification optional.

**Notes:**

WhatsApp notification is optional. The existing email notification behavior remains unchanged for customers who do not specify a WhatsApp number.

**Source Branch:** Feature branch created from the main development branch.

**Destination Branch:** Main development branch.

**PR Reviewers:** Anurag N, Prem Pedamallu

