 Apache Airflow One Shot - ETL Pipeline Using Airflow & Astro  

## 📌 Project Overview  
This project builds an end-to-end ETL (Extract, Transform, Load) pipeline using **Apache Airflow** and **Astro**. It extracts weather data from an API, transforms it, and loads it into PostgreSQL using Docker and Airflow.

##  Features  
- Extracts weather data from **Open-Meteo API**.  
- Transforms data (temperature, wind speed, direction, etc.).  
- Loads processed data into **PostgreSQL**.  
- Uses **Docker & Astro** for containerized execution.  

##  Technologies Used  
- **Apache Airflow**  
- **Astro CLI**  
- **Docker**  
- **PostgreSQL**  
- **Python**
- 
How It Works  
1. **Setup Astro & Docker**  
   - Install Astro CLI (`winget install -e --id Astronomer.Astro`).  
   - Initialize the project (`astro dev init`).  

2. **Define the ETL Pipeline**  
   - Create `etlweather.py` inside `dags/`.  
   - Define Airflow tasks: `extract`, `transform`, `load`.  

3. **Run the Pipeline**  
   - Start Airflow (`astro dev start`).  
   - Check DAGs in **Airflow UI** (`localhost:8080`).  

4. **Data Storage**  
   - Connect **PostgreSQL** (via `docker-compose.yml`).  
   - Verify stored data in the database.  

##  Results  
- Successfully automated data extraction, transformation, and storage.  
- Scalable ETL pipeline with **Airflow DAGs**.
