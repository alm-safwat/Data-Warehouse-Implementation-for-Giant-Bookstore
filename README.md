# Project Summary: Data Warehouse Implementation for Giant Bookstore

I spearheaded a comprehensive data analysis initiative for a prominent giant bookstore client, with the objective of empowering data-driven decision-making. The existing Online Transaction Processing (OLTP) system of the client demanded a robust solution for extracting valuable business insights. In response, I meticulously designed and implemented a data warehouse, choosing a galaxy schema to adeptly manage two distinct fact tables—sales and order delivery status.


![Ssms_D8rvRIpM1h](https://github.com/alm-safwat/galaxy_schema/assets/135442913/789487fc-0322-466e-9d67-fc2ccfc0fe26)


## Unique Challenge

This project posed a distinctive challenge by deviating from conventional approaches, necessitating the utilization of a galaxy schema—an innovation from my previous experiences with star and snowflake schemas. Significantly, the order history fact table embraced an accumulated structure, capturing dates associated with six different order statuses: received, pending, in progress, canceled, returned, and delivered.

## Key Steps and Processes

- **Data Warehouse Design:**
  - Implementation of a galaxy schema to accommodate sales and order delivery status fact tables.
  - Adoption of an accumulated structure for the order history fact table.


![dwh_galaxy_schema](https://github.com/alm-safwat/galaxy_schema/assets/135442913/e69fa57c-1bfb-4389-ad60-bb212848f750)


- **ETL Pipeline Development:**
  - Creation of an Extract, Transform, Load (ETL) pipeline leveraging SQL Server Integration Services (SSIS).
  - Seamless transfer of data from diverse OLTP sources to the data warehouse.


![fact_etl_data_flow](https://github.com/alm-safwat/galaxy_schema/assets/135442913/b6bbd323-c2dc-4cd2-aaa1-af2f57575e30)


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
    

![PBIDesktop_tRcN1vNHhT](https://github.com/alm-safwat/galaxy_schema/assets/135442913/6be16ba5-f281-4408-b325-777fb9fe1a9b)


## Outcome

The successful completion of this integrated solution provides the giant bookstore client with a solid foundation for informed decision-making. The data insights derived from the data warehouse, coupled with Power BI visualizations, contribute to a powerful toolset for strategic and operational decision support.
