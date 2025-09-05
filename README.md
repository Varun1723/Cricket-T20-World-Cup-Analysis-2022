# Cricket-T20-World-Cup-Analysis-2022

### T20 Cricket Team Selection Dashboard 🏏

This project is a dynamic Power BI dashboard designed to assist in selecting the optimal T20 cricket team. By analyzing player performance metrics and applying specific criteria for different player roles (e.g., openers, anchors, all-rounders), the dashboard provides data-driven insights to build a strong and balanced team.

---

### Project Overview 🚀

The objective of this project was to develop an interactive dashboard that simplifies the complex process of team selection. It leverages detailed cricket data to identify players who meet predefined performance benchmarks. The dashboard allows for the comparison of players and the evaluation of potential team compositions.

---

### Data Sources & Preparation 🧹

This project utilized a multi-step data collection and preprocessing pipeline to ensure the data was accurate and ready for analysis.

1.  **Web Scraping**: I used a web scraping tool to extract raw data on player statistics, match results, and other relevant information from various online cricket data sources. The data was scraped in JSON format.
2.  **Data Preprocessing**: The raw JSON data was messy and nested, requiring a robust preprocessing step. I used a **Jupyter notebook** (`t20_data_preprocessing.ipynb`) to clean, transform, and structure the data into a usable format. This involved:
    * Parsing the JSON files to flatten the data.
    * Extracting key player attributes and performance metrics.
    * Creating structured CSV files for easy ingestion into Power BI.
    * The notebook also includes logic to define custom batting orders and calculate boundary runs, as seen in the code snippets.

---

### Data Modeling & Analysis 📊

The core of the project lies in the data modeling and analytical work performed within Power BI.

* **DAX Measures & Calculated Columns**: I created numerous **DAX (Data Analysis Expressions)** measures and calculated columns to derive meaningful insights from the prepared data. These include:
    * `Total Runs`, `Strike Rate`, `Batting Average`, and `Boundary %`.
    * Calculated columns like `boundary runs` to aggregate boundary data.
    * A list of key measures and their formulas can be found in `DAX Measures and Calculated columns.xlsx`.

* **Parameter Scoping**: A key component of this project was defining **player archetypes** based on specific performance criteria. I used a `Parameter Scoping.pdf` document to establish these rules, which were then implemented as filters and visualizations in Power BI. This allows the user to filter players based on roles such as **Openers**, **Anchors**, **Finishers**, and **All-rounders**.

---

### Dashboard Features ✨

The Power BI dashboard offers a range of interactive features to support team selection:

* **Dynamic Filtering**: Users can filter players based on a variety of metrics like batting average, strike rate, and batting position to identify suitable candidates for different roles.
* **Role-Based Player Selection**: The dashboard uses the predefined criteria to highlight players who fit specific roles, making it easy to build a balanced team. 
* **Player Comparison**: Users can select and compare individual players or a combination of players to analyze their strengths and weaknesses side-by-side.

---

### Technologies Used 🛠️

* **Data Collection**: Web scraping tools
* **Data Transformation**: Jupyter Notebook (Python, Pandas)
* **Data Visualization & Analysis**: Power BI (DAX, Power Query)