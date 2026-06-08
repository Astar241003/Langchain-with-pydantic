# LangChain Structured Output Example

A simple example project demonstrating how to use **LangChain**, **Google Gemini**, and **Pydantic** to extract structured information from natural language and apply business validation rules.

## Features

* Natural language data extraction using Gemini
* Structured output with Pydantic models
* Field validation and type enforcement
* Salary normalization (monthly to yearly)
* Loan eligibility calculation
* Unique application ID generation
* CSV-based data storage
* Environment variable management with dotenv

## Tech Stack

* Python
* LangChain
* Google Gemini
* Pydantic
* Pandas
* python-dotenv

## Workflow

```text
User Input
    ↓
Gemini LLM
    ↓
LangChain Structured Output
    ↓
Pydantic Validation
    ↓
Business Logic
    ↓
CSV Storage
```

## Example Use Case

Input:

```text
Rahul Sharma works as a Software Engineer at ABC Technologies.
Salary: 60000 PM
Loan Amount: 250000
Email: rahul@example.com
```

Output:

```json
{
  "application_id": "...",
  "full_name": "Rahul Sharma",
  "email": "rahul@example.com",
  "post": "Software Engineer",
  "company_name": "ABC Technologies",
  "salary_per_year": 720000,
  "loan_amount": 250000,
  "loan_eligibility": "T"
}
```

## Installation

```bash
pip install pandas python-dotenv pydantic langchain langchain-google-genai
```

## Environment Setup

Create `api.env`:

```env
api_key=YOUR_GEMINI_API_KEY
```

## Learning Objectives

This project demonstrates:

* LangChain structured output
* Pydantic model validation
* LLM-to-database workflows
* Business rule implementation using AI-generated data
* Practical GenAI application development

```
```
