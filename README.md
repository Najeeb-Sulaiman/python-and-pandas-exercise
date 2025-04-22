# Airbnb Data Deep Dive – Python + Pandas Challenge

## Overview  
You've learned the core concepts of Python and Pandas, now it's time to apply them to a real-world dataset. This challenge will test your ability to clean, transform, and analyze a complex dataset using only Python and Pandas.

You’ll be working with Airbnb listing data from a major city. Your goal is to uncover patterns, clean messy data, create insightful summaries, and answer key analytical questions using only Pandas.

---

## Dataset  
Download Airbnb data for a city of your choice from [Inside Airbnb](http://insideairbnb.com/get-the-data.html). Cities like **New York City** or **London** are ideal due to their large dataset sizes and variety.

You’ll primarily be working with the `listings.csv` file.

---

## Project tasks

### 1. Data Loading and Initial Exploration
- Load the dataset using Pandas.
- Display basic information (`.info()`, `.describe()`, `.head()`).
- Check for missing values, duplicated rows, and unusual data types.

---

### 2. Data Cleaning
- Convert price fields (e.g., `"$2,100.00"`) to float.
- Parse dates (e.g., `last_review`) into datetime objects.
- Handle missing values in critical fields like `reviews_per_month`, `host_name`, and `neighbourhood_group`.
- Remove or impute irrelevant rows (e.g., listings with zero availability or price).

---

### 3. Data Enrichment
- Create a `price_per_person` column using `price` and `accommodates`.
- Create a `is_superhost` flag from `host_is_superhost`.
- Bucket availability into categories:
  - **Full-time** (availability > 300)
  - **Part-time** (100–300)
  - **Rare** (<100)

---
