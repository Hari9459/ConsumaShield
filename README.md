# ConsumaShield: End-to-End Data Engineering System
This project is a real-time data engineering pipeline designed to collect, process, and store public consumer product recall data. It uses Kafka, Airflow, Spark, Postgres, and Docker. 



## Overview

1. Data Streaming: Initially, data is streamed from the API into a Kafka topic.
  
2. Data Processing: A Spark job then takes over, consuming the data from the Kafka topic and transferring it to a PostgreSQL database.
   
3. Scheduling with Airflow: Both the streaming task and the Spark job are orchestrated using Airflow. While in a real-world scenario, the Kafka producer would constantly listen to the API, for demonstration purposes, we'll schedule the Kafka streaming task to run daily. Once the streaming is complete, the Spark job processes the data, making it ready for use by the LLM application.

All of these tools will be built and run using docker, and more specifically docker-compose.

![chatuml-diagram](https://github.com/HamzaG737/data-engineering-project/assets/71135893/ce92b731-038a-4d9c-9722-f97a6ba51153)

## Maintainer Information

* **Name:** Hari Murukutla
* **Email:** [murukutlahari1999@gmail.com](mailto:murukutlahari1999@gmail.com)
* **Phone:** +1 315 601 0686
* **LinkedIn:** [linkedin.com/in/hari-murukutla](https://linkedin.com/in/hari-murukutla)
* **GitHub:** [github.com/Hari9459](https://github.com/Hari9459)
# ConsumaShield
