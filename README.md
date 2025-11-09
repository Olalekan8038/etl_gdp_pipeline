# GDP ETL Data Pipeline

This project demonstrates an **end-to-end ETL (Extract, Transform, Load) data pipeline** built using Python.  
The pipeline scrapes GDP data from a public Wikipedia page, transforms and cleans the dataset, and loads the final structured data into a **SQLite database** for storage and querying.  

---

## 🛠️ Technologies Used
- Python  
- Pandas  
- BeautifulSoup (Web Scraping)  
- SQLite (Database)  
- Requests  

---

## 📊 Data Source
**Wikipedia – List of Countries by GDP (Nominal)**  

The dataset contains GDP figures for multiple countries along with related economic information.  

---

## 🔄 ETL Workflow

1. **Extract**: Scrapes GDP data from the Wikipedia page using BeautifulSoup and Requests.  
2. **Transform**: Cleans and processes the data using Pandas and NumPy, including removing commas, converting types, and rounding GDP values to billions.  
3. **Load**: Saves the transformed data to a CSV file and inserts it into a SQLite database.  
4. **Query**: Demonstrates basic SQL queries on the loaded data to retrieve insights (e.g., countries with GDP above 100 billion USD).  

---

## ▶️ How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Olalekan8038/etl_gdp_pipeline.git
   cd etl_gdp_pipeline
2. install dependencies 
pandas
numpy
beautifulsoup4
requests
3. Run the ETL pipeline 
python gdp_etl_pipeline.py
4. open the SQLite database to Query the data:
sqlite3 World_economies.db
5. Check the CSV output in the path defined in the script.
## Output sample below:

|  Country       | GDP_USD_billions|
|----------------|-----------------|
| United States  | 25000.0         |
| China          | 18000.0         |
| Japan          | 4500.0          |