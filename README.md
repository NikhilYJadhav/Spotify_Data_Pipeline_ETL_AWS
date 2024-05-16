Business Problem

We have a client who is pationate about music industry and he wants to understand by collecting different data. So, he can find different pattern and make decision based on that.

In spotify we have multiple playlist availabe and for startes our client wants to start the top global song every single weeks. 

So, that he can understand what songs, Album are trending and artist.

All of this will be extracting from sportify api. For this we have Build ETL pipeline on all of Spotify data.

What is ETL?
![ETL](https://github.com/NikhilYJadhav/Spotify_Data_Pipeline_ETL_AWS/assets/112622476/81ea337f-ff88-438f-a623-70780b683c79)

After This Deploy Code on AWS Lambda on top of that we have applied CLoud watch Trigger to run code every week bases or day as per requirement. 

Trigger will run the lambda function extract the api and store the data in S3 Bucket. 

Once data is stored in S3 Bucket, I have applied some lambda transformation code to tranform the data Automatically.

Crawler will go through each of the file what all column, name and data it will understand the data as it is and it will build glue catalog.

AWS Glue Catalog is information of data. After this I have use service Athena which is SQL query to analyze the data.

![AWS](https://github.com/NikhilYJadhav/Spotify_Data_Pipeline_ETL_AWS/assets/112622476/95f188cc-043e-4b66-8e2e-47c052820999)

