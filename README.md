# Random User Data Pipeline

## Project Overview

This project implements a basic Extract, Transform, Load (ETL) pipeline in Python. It demonstrates how to fetch data from an external REST API, perform necessary data cleaning and transformations using the `pandas` library, and then load the processed data into a local SQLite database for structured storage and querying.

The primary goal is to showcase fundamental data engineering skills, including API integration, data manipulation, basic data modeling, and database interaction.

## Features

*   **Data Extraction:** Fetches a specified number of random user profiles from the [Random User Generator API](https://randomuser.me/api/).
*   **Data Transformation:**
    *   Parses and flattens nested JSON data into a clean, tabular format.
    *   Selects relevant user attributes (e.g., first name, last name, email, city, country, age).
    *   Converts data types for better usability (e.g., date strings to date objects, age to integer).
*   **Data Loading:** Stores the transformed data into an SQLite database table.
*   **Data Verification & Querying:** Performs basic SQL queries on the loaded data to ensure integrity and demonstrate data retrieval capabilities (e.g., total records, records by gender).

## Technologies Used

*   **Python 3.10+**: The core programming language.
*   **`requests` library**: For making HTTP requests to the Random User Generator API.
*   **`pandas` library**: For efficient data manipulation, transformation, and DataFrame management.
*   **`sqlite3` (built-in)**: For creating and interacting with the local SQLite database.

## Setup and Installation

Follow these steps to set up and run the project locally.

### Prerequisites

*   Python 3.10 or higher
*   `pip` (Python package installer)

### 1. Clone the Repository

First, clone this GitHub repository to your local machine:

```bash
git clone https://github.com/YourUsername/Random-User-Data-Pipeline.git
cd Random-User-Data-Pipeline
