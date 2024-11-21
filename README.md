# PEMSF_Project
This repo includes the test and training data based on the PEM_SF UCI Machine learning dataset, and our current code to train a model on it.
The PEMS_train data file was too large to upload onto gitlab, even with it is compressed.
You can download a copy of the PEMS_train data file here: https://drive.google.com/file/d/1i7nslTRzBPUx9lnWxKlVTn0ZkQF79icA/view?usp=sharing
We created our model in the python file, project_group2.ipynb.
In order to run project_group2.ipynb, you will need to down load PEMS_train from the google doc link above and move it into the same directory as the the python file.
Next, you will have to download project_group2.ipynb, PEMS_trainlabels.txt, PEMS_test.txt, and PEMS_testlabels.txt as well.
Make sure those files are in the same directory as project_group2.ipynb.
Now you can run project_group2.ipynb.

# PEMSF_Project Prototype
In order to run our project prototype, you need to download the following files, Group2_Project_Prototype.ipynb, PEMS_test.txt, PEMS_trainlabels.txt, First_Day_Guess_label.txt, First_Day_Guess_test.txt, Second_Day_Guess_label.txt, Second_Day_Guess_test.txt, Third_Day_Guess_label.txt, and Third_Day_Guess_test.txt.
Make sure all of the files are in the same directory when you run the python file, Group2_Project_Prototype.ipynb.

# Future Work Data Extraction
The python file, Project_Data_Extractions.ipynb, extracts occupancy rate data from https://pems.dot.ca.gov. First, you will need to create account on https://pems.dot.ca.gov. Once the account is made on line 110 and 111 in the python file, Project_Data_Extractions.ipynb, you will need to input the username and password you just made. Next, you will need to download the file, stations_list.txt. The text consist of all of the sensor IDS used in collecting the original training dataset. Make sure the text file is in the same directory as Project_Data_Extractions.ipynb.
Now you can run Project_Data_Extractions.ipynb.
It will collect occupancy rate sensor data and pre-process it into a text file call self_test.txt.
As an FYI, the python file, Project_Data_Extractions.ipynb is still a work in progress to automatic the whole process of collecting and organizing the data into format our model can read.
