# Realtime Data Streaming | End-to-End Data Engineering Project

This project is a streaming data pipeline that crawls data from a random user API, processes it in real time, and stores the results in a Cassandra database.

## Table of Contents

- [System Architecture](#system-architecture)
- [Built With](#built-with)
- [Getting Started](#getting-started)

## System Architecture

![System Architecture Diagram](Architecture.png)

Our project features a multi-layered streaming data pipeline designed for seamless data flow and robust performance. It all begins with the randomuser.me API, which provides the random user data that kickstarts the process. Apache Airflow then takes charge of orchestrating the entire pipeline, ensuring data is efficiently collected and temporarily stored in a PostgreSQL database. From there, Apache Kafka—supported by Apache Zookeeper—transfers the data to our processing engine, while a dedicated Control Center and Schema Registry keep a close watch on stream integrity and schema consistency. Finally, Apache Spark processes the data using its master-worker model, and the refined results are stored in Cassandra, offering a scalable solution for high-volume data storage.


## Built With

List the main tools, frameworks, or libraries used in your project:

- **Apache Airflow:** Setting up a data pipeline with Apache Airflow.
- **Apache Kafka:** Real-time data streaming with Apache Kafka.
- **Apache Zookeeper:** Distributed synchronization with Apache Zookeeper.
- **Apache Spark:** Data processing techniques with Apache Spark.
- **Cassandra & PostgreSQL:** Data storage solutions using Cassandra and PostgreSQL.
- **Docker:** Containerizing your entire data engineering setup with Docker.



## Getting Started

Follow these instructions to get a local copy of the project up and running:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/yourproject.git
