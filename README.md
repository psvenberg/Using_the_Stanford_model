The MOTOR-t-base model requires an older version of python and older versions of several libraries in order to run successfully. It took me a bit of work to troubleshoot these issues, so I created this repo to share how to make this work. I got the model to work in the Colab environment. 

The "MOTOR_run.ipynb" file contains the code to upload the MOTOR-t-base model into the colab environment. It also contains the code to create realistic but simulated patients to subsequently feed into the model. I created 2 simulated patients to show the general principles of code that can generate these patients. 

The model recognizes patient information only if it is formatted in a specific way. Diagnoses can be assigned to patients using SNOMED codes. Vitals and labs are formatted as LOINC codes. Medications are entered as RxNorm codes (https://mor.nlm.nih.gov/RxNav/ can be used to look up the RxNorm codes for specific medications). The "motor_dictionary_codes.txt" file contains all the codes the model can recognize when creating patient embeddings. The cell in "MOTOR_run.ipynb" that makes simulated patients shows how these codes can be used. 

