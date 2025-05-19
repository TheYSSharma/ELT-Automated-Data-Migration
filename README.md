# ELT-Automated-Data-Migration
Complete End to End Automated ELT Data Migration from Source Database to Destination Database
1. Data is extracted from the source_db - Postgres.
2. The Extracted data is then loaded in a destination_db - Postgres.
3. The Extraction and Loading of data is done using the ELT_sript file.
4. Once the data is loaded into the destinaion_db it is them transform for using DBT as per the requirement by other data teams.
5. A CRON job is created and this CRON job performs the data migration process. This CRON Job is scheduled to run exactly at 3.00 am.
6. 
