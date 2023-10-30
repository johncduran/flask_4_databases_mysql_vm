# flask_4_databases_mysql_vm
HHA 504 4b

## Schema Azure
I created a new database in MySQL Workbench called 'AzureVM' and created three tables within it. In the patient_medications table there is a foreign key of patient_id form the patients table and a foreign key of medication_id from the medications table. I also added a new user named johncd to see if I could grant it access to the entire database.

## Schema GCP
I was not able to get MySQL Workbench to connect to the GCPVM as it kept saying that it was failing to connect. However, if I was able to get it to connect then I would've used the same schema that I used on the Azure VM.

## Flask Implementation
After creatign the app.py file I added in the appropiate libraries such as os, dotenv, pandas and sqlalchemy. I then added the connection string to connect to the Azure VM by allowing it to access the necessary information in the .env file that I created. This contained variables such as the database username, password, port and more. 

## Errors 

In Azure I faced errors when it came to creating the databases in MySQL Workbench. I was able to create a new database called Azure. However, I did have issues with selecting that same database as it was "Error Code: 1046. No database selected Select the default DB to be used by double-clicking its name in the SCHEMAS list in the sidebar."


In GCP I was unable to get access to login to the GCPVM as it would say that I didn't have permission. I did add a new firewall rule for port 3306, but that still didn't give me access.
