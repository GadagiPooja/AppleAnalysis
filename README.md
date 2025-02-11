# ETL Pipeline with Apache Spark

## Project Overview
This project implements an ETL (Extract, Transform, Load) pipeline using Apache Spark to generate customer data insights based on their purchasing behavior. The pipeline identifies customers who have:
1. Bought AirPods just after buying an iPhone.
2. Bought only an iPhone and AirPods.

## Technologies Used
- **Apache Spark** (for distributed data processing)
- **Python** (for ETL scripting)
- **Pandas** (for data handling and transformation)
- **AWS S3 / HDFS** (for storage, if applicable)
- **PostgreSQL / MySQL** (for data persistence, if applicable)

## Project Structure
```
ETL_Project/
│── src/
│   ├── first_workflow.py    # Pipeline for customers who bought AirPods after iPhone
│   ├── second_workflow.py   # Pipeline for customers who bought only AirPods and iPhone
│   ├── workflow_runner.py   # Main entry point to execute workflows
│   ├── extractors.py        # Handles data extraction
│   ├── transformers.py      # Implements transformation logic
│   ├── loaders.py           # Handles data loading
│── data/                    # Sample data files (if applicable)
│── README.md                # Project documentation
│── requirements.txt         # Required dependencies
```

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/GadagiPooja/AppleAnalysis.git
   cd ETL_Project
   ```
2. Create a virtual environment (optional but recommended):
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```
3. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```



## Workflows
1. **FirstWorkFlow**: Extracts data, identifies customers who purchased AirPods after an iPhone, and loads the data into a sink.
2. **SecondWorkFlow**: Extracts data, filters customers who purchased only an iPhone and AirPods, and loads the data into a sink.





## Author
Pooja Gadagi
