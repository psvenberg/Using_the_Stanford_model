The MOTOR-t-base model requires an older version of python and older versions of several libraries in order to run successfully. It took me a bit of work to troubleshoot these issues, so I created this repo to share how to make this work. I got the model to work in the Colab environment. 

The "MOTOR_run.ipynb" file contains the code to upload the MOTOR-t-base model into the colab environment. It also contains the code to create realistic but simulated patients to subsequently feed into the model. I created 2 simulated patients to show the general principles of code that can generate these patients. 

The "motor_dictionary_codes.txt" file contains the codes the model can recognize to create patient embeddings. The cell in "MOTOR_run.ipynb" that makes simulated patients shows how to use these codes. Diagnosis codes can be ICD or SNOMED codes. Vitals and medications are formatted as LOINC codes. See the cell to understand the formatting better. 

