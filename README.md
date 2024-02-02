# Project Summary: Data Warehouse Implementation for Giant Bookstore

I spearheaded a comprehensive data analysis initiative for a prominent giant bookstore client, with the objective of empowering data-driven decision-making. The existing Online Transaction Processing (OLTP) system of the client demanded a robust solution for extracting valuable business insights. In response, I meticulously designed and implemented a data warehouse, choosing a galaxy schema to adeptly manage two distinct fact tables—sales and order delivery status.

## Unique Challenge

This project posed a distinctive challenge by deviating from conventional approaches, necessitating the utilization of a galaxy schema—an innovation from my previous experiences with star and snowflake schemas. Significantly, the order history fact table embraced an accumulated structure, capturing dates associated with six different order statuses: received, pending, in progress, canceled, returned, and delivered.

## Key Steps and Processes

- **Data Warehouse Design:**
  - Implementation of a galaxy schema to accommodate sales and order delivery status fact tables.
  - Adoption of an accumulated structure for the order history fact table.

- **ETL Pipeline Development:**
  - Creation of an Extract, Transform, Load (ETL) pipeline leveraging SQL Server Integration Services (SSIS).
  - Seamless transfer of data from diverse OLTP sources to the data warehouse.

- **Dimension Management:**
  - Implementation of slowly changing dimensions to address dynamic changes in dimension attributes.
  - Assurance of data integrity through effective management of evolving dimensions.

- **Source System Identification:**
  - Introduction of a "source_system_code" column in the data warehouse for categorizing data based on its origin.
  - Categorization of data to accommodate the client's multiple branches.

- **Metadata Control Table:**
  - Creation of a "meta data control table" to streamline data flow control.
  - Storage of critical information, including the last load date, facilitating seamless continuation of subsequent data loads.

- **Power BI Integration:**
  - Utilization of Power BI for comprehensive data analysis and visualization.
  - Tailoring Key Performance Indicators (KPIs) to meet the specific business requirements of the giant bookstore client.
![PowerBI_Performance_Tracker](https://github.com/alm-safwat/galaxy_schema/assets/135442913/d7016f5e-ef28-4000-bd2c-48021bb429a8)

## Outcome

The successful completion of this integrated solution provides the giant bookstore client with a solid foundation for informed decision-making. The data insights derived from the data warehouse, coupled with Power BI visualizations, contribute to a powerful toolset for strategic and operational decision support.
