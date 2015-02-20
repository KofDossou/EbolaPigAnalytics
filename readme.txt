
Description:
===========
(Source: cdc.gov) Ebola is a rare and deadly disease caused by infection with a strain of Ebola virus.
The 2014 Ebola epidemic is the largest in history, affecting multiple countries in West Africa.
The metadata used in this analysis spans a series of African countries affected by the deadly Ebola virus.
The analytics performed on this data evolves around the  locality of the countries, the category and the value. 
A country can have different localities which report varying number of category of cases and value.



Data Processing Activities:
=====================================
Step 1: Downloaded Ebola Metadata from http://www.google.com/publicdata/explore?ds=eq10po6kah9si_&hl=en_US&dl=en_US	
Step2: Setup 4 instances of AWS(amazon Web Services) EC2 lunched via Ubuntu Server 14.04 LTS (HVM)
Step3: Assigned Master and Slaves nodes (secondary node, slave 1 &2)
Step4: Enable SSH capabilities via Master node to all slave nodes using key pair obtained from AWS
Step5: Downloaded: Java, Hadoop on all nodes. Downloaded Pig on Master node only.
Step6: Created Folder (ebola.txt) in unix via vi and moved copied ebola metadata into it .
Step7: Moved ebola.txt to hdfs (hadoop distribution file system)
Step8: Start pig engine (grunt> ) at terminal tells as pig is working properly
Step9: set path to hdfs
Step10: write and execute script

Tools:
========
Amazon EC2 5 instances (master, secondary and salve 1,2&3)
Ubuntu server
Java 
Hadoop 
Pig Latin







