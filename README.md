# Using Bashscripts to Upload to a GCP Bucket 


# Overview 
This short script will allow you to upload a file(s) in your current directory to a GCP storage bucket. This script assumes you have the GCP SDK installed on your local device and that you have sufficient privilages to create a storage bucket and upload files to that bucket (Cloud Storage Editor Role). 

The user should also have the ability execute the script in the bash shell. You may need to edit user permissions on the script by running the chmod command. 

# Requirements 
1. Cloud SDK installed on your device
2. A GCP project 
3. Cloud Storage Editor Role or the required permissions to: create and list storage buckets. read/write to that bucket. 
4. Permission to execute the bash script on your device 

# Directions 
Run the script in the same directory as the files you wish to upload. You can enter the file(s) that you would like upload as follows: 

`./gcpscript [file1] [file2] ...`

The script will first authenticate your GCP account and you will follow each prompt to select your desired GCP configuration. Once authenticated, the available storage buckets in the current project will be listed and you will be given a choice to upload to an existing bucket or create a new storage bucket. The script will check that the files you provided exist and will then display a message if the upload was successful. 

