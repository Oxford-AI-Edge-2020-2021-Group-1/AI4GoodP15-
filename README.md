# Oxford's AI Group 1's solution to Project 15's ELP Repo

## Members of Group 1 include:
Rick Durham, Srikar Vedula, Sukanya Mandal, Thanya Chartsakulkanajarn, Oscar Ordenes, Harnaik Nahal. 

# Introduction
Microsoft's Project 15 approached Oxford University's AI group to work on objectives outlined on the P15 Challenge document (https://docs.google.com/document/d/1kMtjQrvL-XOqQCncvaZfVceHBbB6Vqxz/edit). Upon discussion, Group 1 has decided to further the development of gunshot identification and classification in the ELP audios. 

# Problem analysis / Data preview
A variety of ELP audios from different geographical areas were obtained and placed into a directory to work in MATLAB 2020b. Snippets needed to be collated as the 1.3Gb of 24hours of audio were to large to be analysed at once. The Audio Toolbox was heavily used. MATLAB code included in the features folder. 

main_v2 is the mean live script. 
getAudio and getData help compile big audio files into smaller snippets. 

# Modelling
The audio datasets are located under code/datsets/readme.md where the google drive link is provided. Since the files size is too huge, we could not upload the audio files into github. Under the google drive link, download the raw_audio_training_dataset and raw_audio_testing_dataset. Each one contains a zip folder for all the training and testing audio files. Save the training audio files and testing audio files in separate directories. Keep the train.csv and test.csv in the same directory as the model. The model can be found under code/models/project15finalmodel.py. Change the directories of where you has saved the training audio files, testing audio files, train.csv, test.csv and the directories of where the spectrogram images will be saved once you run the model. The model itself will take 20-30 minutes to run as it needs to conver the audio files into spectrograms and then compile the model. Take several audio files and save them into a seperate directory where you will test/evaluate the model. 

# Get started.
Please view this video (https://drive.google.com/file/d/1_p6-_vdX0RQ0xff_PhFb6Tqz2CYR968U/view?usp=sharing)_ for more information on our work.

# Contributing
More documentation on our work can be found here along with our information if you would like to contact us to collaborate! (https://sway.office.com/BAUOcURUXpxB3BTu). On there you can find our LinkedIn profiles and reach out to us there!

# Default Directory Structure

```
├── .cloud              # for storing cloud configuration files and templates (e.g. ARM, Terraform, etc)
├── .github
│   ├── ISSUE_TEMPLATE
│   │   ├── Ask.md
│   │   ├── Data.Aquisition.md
│   │   ├── Data.Create.md
│   │   ├── Experiment.md
│   │   ├── Explore.md
│   │   └── Model.md
│   ├── labels.yaml
│   └── workflows
├── .gitignore
├── README.md
├── code
│   ├── datasets        # code for creating or getting datasets
│   ├── deployment      # code for deploying models
│   ├── features        # code for creating features
│   └── models          # code for building and training models
├── data                # directory is for consistent data placement. contents are gitignored by default.
│   ├── README.md
│   ├── interim         # storing intermediate results (mostly for debugging)
│   ├── processed       # storing transformed data used for reporting, modeling, etc
│   └── raw             # storing raw data to use as inputs to rest of pipeline
├── docs
│   ├── code            # documenting everything in the code directory (could be sphinx project for example)
│   ├── data            # documenting datasets, data profiles, behaviors, column definitions, etc
│   ├── media           # storing images, videos, etc, needed for docs.
│   ├── references      # for collecting and documenting external resources relevant to the project
│   └── solution_architecture.md    # describe and diagram solution design and architecture
├── environments
├── notebooks
├── pipelines           # for pipeline orchestrators i.e. AzureML Pipelines, Airflow, Luigi, etc.
├── setup.py            # if using python, for finding all the packages inside of code.
└── tests               # for testing your code, data, and outputs
    ├── data_validation
    └── unit
```
