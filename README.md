NoSQL Databases with MongoDB

## Overview

This module dives into the use of NoSQL databases, specifically MongoDB, for managing and analyzing unstructured data. Unlike traditional SQL databases, MongoDB offers greater flexibility with JSON-like documents, making it suitable for projects that involve dynamic or hierarchical data.

---

## Lessons

### 12.1 Introduction to NoSQL and MongoDB
- **Learned Concepts:**
  - Differences between SQL and NoSQL databases and their use cases.
  - Setting up and connecting to a local MongoDB instance.
  - Performing basic CRUD operations (Create, Read, Update, Delete).
  - Importing CSV and JSON files into MongoDB.

### 12.2 PyMongo and Advanced Queries
- **Learned Concepts:**
  - Using PyMongo to interact with MongoDB from Python.
  - Retrieving specific fields and filtering data using comparison operators.
  - Sorting and limiting query results.

### 12.3 Aggregation, Analysis, and Integration with MongoDB
- **Learned Concepts:**
  - Creating aggregation pipelines for advanced data analysis.
  - Converting MongoDB results into Pandas DataFrames for further processing.
  - Visualizing data using Matplotlib and integrating APIs for additional insights.

---

## Project: UK Food Standards Agency Database Analysis

### Part 1: Database Setup
1. Imported data from `establishments.json` into a local MongoDB database named `uk_food`.
2. Connected to the database using PyMongo and confirmed the setup by:
   - Listing all databases and collections.
   - Displaying a sample document using `find_one()`.

### Part 2: Updating the Database
- Added a new halal restaurant entry to the database.
- Updated the `BusinessTypeID` field for the new restaurant.
- Removed all establishments in Dover.
- Converted string fields (e.g., `latitude`, `longitude`, and `RatingValue`) into appropriate numerical formats.

### Part 3: Exploratory Analysis
- Answered key questions to help "Eat Safe, Love" identify suitable establishments:
  1. Found establishments with a hygiene score of 20.
  2. Identified establishments in London with a `RatingValue` ≥ 4.
  3. Retrieved the top 5 establishments near "Penang Flavours" with the lowest hygiene scores.
  4. Aggregated data to rank Local Authority areas by the number of establishments with a hygiene score of 0.

---

## Tools Used
- **MongoDB**: For storing and managing NoSQL data.
- **PyMongo**: Python library for interacting with MongoDB.
- **Pandas**: For converting MongoDB data into tabular formats.
- **Matplotlib**: For visualizing analytical results.

---

## Skills Gained
- Differentiating SQL and NoSQL databases.
- Performing CRUD operations in MongoDB.
- Writing aggregation pipelines for advanced queries.
- Visualizing and integrating MongoDB data with Python tools.
