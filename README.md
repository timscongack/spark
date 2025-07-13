# Local Spark Cluster with Docker

This repository provides a local Spark cluster setup using Docker Compose, and examples/code of my walkthrough of Spark's Definitive Guide by Bill Chambers and Matei Zaharia.

## Getting Started

### 1. Install Docker Desktop

### 2. Start the Spark Cluster

```bash
docker-compose up -d
```
- Spark Master UI: http://localhost:8080
- Jupyter Lab: http://localhost:8888

### 3. Run an Example Operation

Use `spark-submit` inside the master container. For example, to run the basic CSV read example:

```bash
docker exec -it spark-master spark-submit \
  --master spark://spark-master:7077 \
  /opt/bitnami/spark/examples/transformations/01-basics/read_flight_csv.py
```

---

This example demonstrates how to read a CSV file using Spark DataFrame API.

## How to Run

```bash
docker exec -it spark-master spark-submit \
  --master spark://spark-master:7077 \
  /opt/bitnami/spark/examples/transformations/01-basics/read_flight_csv.py
```

The script reads the `data/flight-data/csv/2010-summary.csv` file and prints the first 5 rows. 