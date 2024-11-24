# Part 1: PEM-SF_model
This repo ultilized the PEM-SF dataset from the UCI Machine Learning Repository to develop a training and test dataset as the bases to develop and train a robust traffic classifer model to determine the day-of-week.

# Instructions to run notebook  
1. Download the zip file.
2. Extract and save the files.
3. Upload the files onto your notebook.
4. Ensure all files are in the same directory prior to running the script.
5. Run code.

        # Files to run our PEMS-SF Traffic Classifer Model:
            1. PEMS-SF_model.ipynb
            2. PEMS_train.txt
            3. PEMS_trainlabels.txt
            4. PEMS_test.txt
            5. PEMS_testlabels.txt
       

# Part 2: PEMS-SF_prototype
This prototype classifies the day-of-week based on specific traffic inputs (must contain 963 features and 144 time dimensions).

# Instructions
Follow the steps above ("Instructions to run notebook") if not completed earlier. 

        # Files to ulitlize for PEMS-SF_prototype.ipynb
            1. PEMS-SF_prototype.ipynb
            2. PEMS_test.txt
            3. PEMS_trainlabels.txt
            4. guess_1_train.txt
            5. guess_1_test.txt
            6. guess_2_train.txt
            7. guess_2_test.txt
            8. guess_3_train.txt
            9. guess_3_test.txt
            10. random_forest_model.pkl


# Part 3: PEMS-SF_extractions <br>
Future Work (Status: WIP) : **NOT A REQUIREMENT FOR THIS PROJECT - REQUIRES PEMS ACCOUNT** <br>
The python file, PEMS-SF_extractions.ipynb, extracts occupancy rate sensor data from https://pems.dot.ca.gov and pre-process it into a text file called self_test_txt. Note that is effort is a work in progress to work in progress to automatic the whole process of collecting and organizing the data into format that is readable by our model.

# Instructions:
1. Complete steps listed above ("Instructions to run notebook") if not done already.
2. Create an account on https://pems.dot.ca.gov (**PEMS username & password required for script**) 
3. In the PEMS-SF_extraction notebook, find the "Set-up access to Caltrans PeMS" section. This will be at the top of the cell. Update the USERNAME and PASSWORD portion of the script to your appropriate credentials.
4. May adjust parameters accordingly to obtain desired information.
5. Run code.

        # Files to perform PEMS-SF extraction
            1. PEMS-SF_extractions.ipynb
            2. stations_list.txt
            

**Disclaimers** 
The given test dataset from PEMS-SF was found to largely comprise of the same data in the training dataset. As a result, the original training dataset was split for ultilization for training, test crossvalidation, testing, and the demo.

An attempt was made to generate our own test dataset from Caltrans PeMS. However, the author for the PEMS-SF did not provide instructions of how the datasets were preprocessed. Dimention reduction with incremental PCA after cleaning and normalization the data was tried but did not generate a test dataset that function desirabilty with the training data. 

It should also be noted that the datasets have been preprocessed. Any attempts of dimentional reduction resulted in a suboptimal F1-score.

Additionally, the author for PEMS-SF stated the numberical dates start with Day 1 = Monday. However, this has been corrected to Day 1 = Sunday to correctly match the information provided by Caltrans PeMS.

# References
Reference to original dataset for this project: https://archive.ics.uci.edu/dataset/204/pems+sf
Cuturi, M. (2011). PEMS-SF [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C52G70.
