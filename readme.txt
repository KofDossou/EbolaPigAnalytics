
Description:
===========
(Source: cdc.gov) Ebola is a rare and deadly disease caused by infection with a strain of Ebola virus.
The 2014 Ebola epidemic is the largest in history, affecting multiple countries in West Africa.
The metadata used in this analysis spans a series of African countries affected by the deadly Ebola virus.
The analysis also includes the locality of the countries, the category and the value. I will be analyzing the Ebola metadata based on African countries affected by the Ebola virus in relation to  their locality, category (cases, death, confirmed/new/suspected, probable cases) and value (number of cases/death recorded) .
A country can have different localities which report varying number of category of cases and value. Due to the vast amount of data in this file, computed output was limited to only 100 outputs. **Limited can be increase if more computed results is desired.
Data Size- 1542kb


Data Processing Activities:
=====================================
Step 1: Downloaded Ebola Metadata from http://www.google.com/publicdata/explore?ds=eq10po6kah9si_&hl=en_US&dl=en_US	
Step2: Setup 4 instances of AWS(amazon Web Services) EC2 lunched via Ubuntu Server 14.04 LTS (HVM), SSD Volume Type - ami-3d50120d
Step3: Assigned Master and Slaves nodes (secondary node, slave 1 &2)
Step4: Enable SSH capabilities via Master node to all slave nodes using key pair obtained from AWS
Step5: Downloaded: Java, Hadoop on all nodes. Downloaded Pig on Master node only.
Step6: Created Folder (ebola.txt) in unix via vi and moved copied ebola metadata into it .
Step7: Moved ebola.txt to hdfs (hadoop distribution file system)
Step8: Start pig engine (grunt> ) at terminal tells as pig is working properly
Step9: set path to hdfs
Step10: write and execute script

