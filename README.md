# ETL Pipeline for Netflix Data Analysis

## Description
This project aims to develop an ETL (Extract, Transform, Load) pipeline to analyze content distribution trends on Netflix. The pipeline is built on AWS, using DBT for data transformation, Snowflake as the data warehouse, and Airflow for orchestration. The insights are visualized using AWS Quicksight, and alert mechanisms are integrated for monitoring pipeline failures.

![Netflix Data Visualization](https://github.com/hxu47/airflow-code/blob/main/image.png)


## Getting Started

### Prerequisites
- AWS EC2 instance
- AWS Snowflake account
- DBT installed
- Apache Airflow installed

### Installation Steps
1. **AWS EC2 Setup**: Launch an EC2 instance on AWS to host DBT and Airflow.
2. **DBT Installation**: Install DBT on the EC2 machine following [DBT Installation Guide](https://docs.getdbt.com/docs/introduction).
3. **Airflow Installation**: Install Apache Airflow following [Airflow Installation Guide](https://airflow.apache.org/docs/apache-airflow/stable/start.html).

## Project Outline
- **Install dbt and Airflow on an AWS EC2 machine.**
  - This is the initial setup step. Instructions can be found in the installation steps section.
- **Create a dbt pipeline for the business use case discussed in this [Project](https://github.com/hxu47/dbt-code).**
  - Run the data transformations required for the analysis.
  - Business Use Cases include:
    - In terms of content, which movies/series dominate the market?
    - Who are the top actors and directors dominating specific genres?
    - Percentage share of movies/series on Netflix's platform.
- **Use Airflow as the orchestrating tool.**
  - Set up DAGs to schedule and automate the pipeline tasks.
- **Automate test cases in the pipeline.**
  - Implement testing to ensure data quality and integrity.
- **Create visualizations using AWS Quicksight.**
  - Transform the processed data into insightful visualizations.
- **Set up alerting mechanisms for pipeline failure using Slack and email alerts.**
  - Monitor the pipeline and receive immediate notifications for any issues.

## How to Use
- Step 1: Start your EC2 instance and connect to your Snowflake account.
- Step 2: Run the Airflow server.
- Step 3: Trigger the DBT transformations via Airflow.
- Step 4: View the Quicksight dashboard for results.
- Step 5: Monitor the pipeline through Slack and email alerts.


