# Stock Market Real-Time Data Pipeline with Apache Kafka & Cassandra

This project centers on the utilization of Python to retrieve live stock market data in real-time, which is subsequently stored in a Cassandra database through Apache Kafka. The data is further processed on an AWS EC2 instance using Apache Kafka and ultimately stored in a local Cassandra server.

## Key Features

- Data Engineering: Develop and implement a robust data pipeline to facilitate the seamless processing of real-time data streams.
- Technology Stack: Employ a comprehensive tech stack encompassing Python, AWS EC2, Apache Kafka, and CassandraDB to optimize the data handling process.
- Error Handling: Implement effective error-handling mechanisms to address typical issues and furnish troubleshooting guidelines, ensuring an uninterrupted workflow.
- Future Advancements: Envision potential future enhancements, such as integrating data visualization, machine learning predictions, real-time alerts, and scalability features to augment the system's capabilities and adaptability.

## Architecture

![Pipeline Architecture](https://github.com/princebhatt9588/Stock_Market_Real_Time_Data_Pipeline_Project_with-Apache-Kafka-and-Cassandra/assets/117750531/db6b6e08-b48b-4381-8338-66c72f52f9d3)

## Environment Setup

### Hardware Used

Local Machine:

```bash
  Ubuntu 22.04.1 LTS
  4 vCore, 4 GiB Memory, 32 GiB Storage
```

AWS EC2:

```bash
  Amazon Linux 2 Kernel 5.10
  t2 Family, 1 vCore, 1 GiB Memory
```

### Prerequisites

Make sure you have the following prerequisites installed:

- Python with `kafka-python` & `cassandra-driver` packages
- AWS CLI
- Java
- Apache Kafka
- Cassandra

## Project Implementation

To execute the project successfully, please adhere to the following steps:

Step 1:
Deploy an EC2 instance and conduct the installation of Apache Kafka.

Step 2:
Develop a Python script to facilitate the retrieval of real-time stock market data.

Step 3:
Leverage Apache Kafka to produce the obtained data to a designated topic.

Step 4:
Generate a Python script aimed at consuming the data from the topic and proficiently storing it within CassandraDB.

## Execution

To effectively execute the project, please adhere to the following steps:

Step 1:
Initiate the launch of an EC2 instance and proceed with the setup of Apache Kafka.

Step 2:
Commence the operation of the Apache Kafka producer to generate and dispatch data to a specified topic.

Step 3:
Execute the Python script responsible for transmitting real-time stock market data.

Step 4:
Commence the operation of the Python consumer script, which will consume the data from the topic and subsequently store it in CassandraDB.

Step 5:
Employ SQL queries to retrieve and access the data stored within CassandraDB for further analysis and processing.

## Error Handling and Troubleshooting

Here are some common errors that may arise during the project execution, along with corresponding troubleshooting tips:

1. Apache Kafka Connection Error:
Error Description: If you encounter difficulties connecting to Apache Kafka, it could be due to issues with the EC2 instance or Apache Kafka service.
Troubleshooting Tips:
   - Verify that the EC2 instance is running and accessible.
   - Check if the Apache Kafka service is running on the EC2 instance.
   - Ensure that the security group settings allow inbound and outbound traffic on the required ports for Kafka communication.

2. Cassandra Connection Error:
Error Description: Facing difficulties connecting to CassandraDB could be attributed to problems with the Cassandra service or firewall settings.
Troubleshooting Tips:
   - Ensure that the Cassandra service is running on the local server.
   - Check the firewall settings to confirm that the necessary ports for Cassandra communication are open.

3. Data Retrieval Error:
Error Description: If issues arise while retrieving stock market data, it might be related to problems with the data retrieval script.
Troubleshooting Tips:
   - Inspect the data retrieval script for any syntax errors or logic issues.
   - Verify that the script has the necessary permissions and access to the required data sources.

4. Data Storage Error:
Error Description: Encountering problems while storing data in CassandraDB might be due to incorrect table configurations or data format issues.
Troubleshooting Tips:
   - Ensure that the required tables have been created in CassandraDB and have the appropriate schema.
   - Check if the data being sent to CassandraDB matches the defined schema for each table.

5. Data Query Error:
Error Description: Facing challenges when querying data stored in CassandraDB may result from erroneous SQL queries or missing tables.
Troubleshooting Tips:
   - Double-check the SQL queries for accuracy and correctness.
   - Verify that the required tables exist in the CassandraDB and that they contain the data you are attempting to query.

By following these troubleshooting tips, you can efficiently address common errors and ensure a smooth workflow throughout the project execution.

## Future Enhancements

- Implementation of a data visualization layer utilizing tools like Matplotlib or Seaborn to graphically present the stock market data stored in CassandraDB.
- Integration of a machine learning model for stock price prediction based on the existing data.
- Deployment of a real-time alert system to promptly notify users of noteworthy stock market changes.
- Scaling of the pipeline's data processing capacity through the addition of more EC2 instances and augmenting the size of CassandraDB clusters.

## Conclusion

This project showcases the utilization of Python, AWS, Apache Kafka, Cassandra, and SQL for the retrieval and storage of real-time stock market data. The developed pipeline can be easily adapted to efficiently process and store various real-time data streams beyond the stock market domain.
