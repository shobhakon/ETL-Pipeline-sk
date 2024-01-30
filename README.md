### INTRODUCTION

Building ETL Pipeline - Task invovled
1. Extract - extracting the data with 400k transactions from Amazon Redshift database.
2. Transform - transform the data by identifying and removing duplicated transactions.
3. Load - load the transformed data to Amazon S3.

### REQUIREMENTS
- Docker

### Coding instructions :
1. Copy the .env.copy file to .envand fill out the environment variables.

2. Ensure your Docker desktop is running.
3. Create the image which contains the execution steps:
   docker image build -t etl.
4. Run the ETL Pipeline using Docker
   docker run --env-file .env etl
