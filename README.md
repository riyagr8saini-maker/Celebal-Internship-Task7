# Pandas Data Cleaning & Exploration Pipeline

## 📌 Objective
This repository demonstrates foundational data manipulation, cleaning, and exploratory data analysis (EDA) using the Python `pandas` library. The project processes a raw retail dataset (Superstore) to ensure data quality, remove inconsistencies, and engineer new features for downstream analysis.

## 🛠️ Technologies Used
* **Language:** Python
* **Libraries:** Pandas
* **Environment:** Google Colab / Jupyter Notebook

## 🚀 Key Data Operations Performed
1. **Data Ingestion & Inspection:** * Loaded raw CSV data and resolved encoding issues.
   * Explored dataset architecture using `.head()`, `.tail()`, `.shape`, and `.dtypes`.
2. **Data Quality Assurance (Cleaning):**
   * Identified and dropped records containing `null` values using `.dropna()`.
   * Ensured dataset uniqueness by removing redundant rows with `.drop_duplicates()`.
3. **Targeted Filtering:**
   * Applied boolean indexing to filter and extract specific subsets of data (e.g., isolating the 'Technology' category).
4. **Feature Engineering:**
   * Derived a new analytical metric: `Total_Amount`. 
   * Calculated by first reverse-engineering the `Unit_Price` (`Sales / Quantity`) and multiplying it by the `Quantity`.
5. **Data Export:**
   * Exported the fully cleaned and augmented dataset to a new CSV file (`cleaned_superstore.csv`) without index duplication.

## 📂 Repository Structure
* `task7.ipynb` - The primary Jupyter Notebook containing the full Python/Pandas code and logic.
* `superstore.csv` - The original, raw dataset.
* `cleaned_superstore.csv` - The finalized dataset post-cleaning and feature engineering.
* `summary.txt` - A detailed text summary of the analytical transformations.

## ⚙️ How to Run
1. Clone this repository to your local machine.
2. Open `task7.ipynb` using Jupyter Notebook or upload it to Google Colab.
3. Ensure `superstore.csv` is located in the same directory.
4. Execute the cells sequentially to reproduce the cleaned dataset.
