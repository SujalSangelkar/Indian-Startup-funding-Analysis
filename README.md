# Indian-Startup-funding-Analysis

This project analyzes startup funding data from `startup_funding.csv` to explore trends, top sectors, cities, startups, and investment types. It uses **pandas** for data manipulation and **matplotlib/seaborn** for visualization.

## 📂 Dataset

The dataset should contain at least the following columns:

* `Date dd/mm/yyyy` – Date of funding.
* `Amount in USD` – Funding amount in USD.
* `Industry Vertical` – Industry category of the startup.
* `City  Location` – City where the startup is located.
* `Startup Name` – Name of the startup.
* `InvestmentnType` – Type of investment.

## ⚙️ Requirements

Install the necessary libraries before running the script:

```bash
pip install pandas matplotlib seaborn
```

## 📜 How It Works

1. **Read the dataset**

   ```python
   df = pd.read_csv('/content/startup_funding.csv')
   ```
2. **Data cleaning**

   * Convert date strings to datetime format.
   * Remove commas from `Amount in USD` and convert to numeric.
3. **Analysis**

   * **Funding Trend** – Monthly total funding amounts.
   * **Top Sectors** – 5 most common industry verticals.
   * **Top Cities** – 5 cities with the most funding.
   * **Top Startups** – 5 startups with the highest funding.
   * **Investment Type Distribution** – Count of each investment type.
4. **Visualization**

   * Line chart of funding trends over time.
   * Bar charts for top sectors, cities, startups, and investment types.

## 📊 Example Visualizations

The script produces:

* **Funding Trend Over Time**
  Line chart showing monthly funding amounts.
* **Top 5 Industry Verticals**
  Bar chart of industries by startup count.
* **Top 5 Cities**
  Bar chart of cities by funding.
* **Top 5 Startups**
  Bar chart of startups by funding.
* **Investment Type Distribution**
  Bar chart of investment types.

## ▶️ Running the Script

Run the script in your terminal:

```bash
python main.py
```

Or in Jupyter/Colab:

```python
!python main.py
```

---
