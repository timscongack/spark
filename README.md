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

### 3. Download Data

The data folder is not included in this repository due to size constraints. You can download the required data files from the official Spark Definitive Guide repository:

**Download data from:** https://github.com/databricks/Spark-The-Definitive-Guide/tree/master/data

Place the downloaded data files in the `data/` directory in your local repository.

### 4. Open Notebooks in VS code/cursor and connect to jupyter kernal at `http://localhost:8888`