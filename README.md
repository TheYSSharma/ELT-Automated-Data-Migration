# ELT-Automated-Data-Migration
Complete End to End Automated ELT Data Migration from Source Database to Destination Database
1. There are 3 separate docker containers made for Source Db, Destionation BD and Postgres files.
2. A Docker Network is created inorder for the above mentioned containers to communicate.
3. Volumes, Images of these containers are stored on the docker and these images are used for the futher ELT Data Migration.
4. Data is extracted from the source_db - Postgres.
5. The Extracted data is then loaded in a destination_db - Postgres.
6. The Extraction and Loading of data is done using the ELT_sript file.
7. Once the data is loaded into the destinaion_db it is them transform for using DBT as per the requirement by other data teams.
8. A CRON job is created and this CRON job performs the data migration process. This CRON Job is scheduled to run exactly at 3.00 am.
9. In the later stages of this projects various dags were created in airflow inorder to schedule and monitor the data migration project
10. Lastly we have used Apache Airflow for orchestration of the entire datapipeline created. 
