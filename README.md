# Bank_Note_Authentication
This Repository is a self taught project in order to learn End to End Deployment of Machine Learning Model.

## This repository contains the following files:
1. BankNoteClassifier(RFC).ipynb
    - This is a Jupyter notebook where the model is trained, tested and saved.

2. [datasets_84803_196262_BankNote_Authentication.csv](https://github.com/azlaanmsamad/Bank_Note_Authentication/blob/master/datasets_84803_196262_BankNote_Authentication.csv) and [Test.csv](https://github.com/azlaanmsamad/Bank_Note_Authentication/blob/master/TestFile.csv)
    - There are the training and test csv files.

3. DockerFile: As the name suggests it is the docker file.

4. bank_note_classifier.pkl
    - The trained classifier model.

## Installation

1. Clone the repository.
2. Build the docker image using the command `docker build -t bank_api`.
3. Run the docker image using the following command in the terminal `docker run -p 8000:8000 bank_api`
4. Open any browser and go to the page `http://0.0.0.0:8000/apidocs`
5. Next click on `GET`, then `Try it out` and finally enter the value for **Variance, Skewness, Curtosis and Entropy.**
6. Finally `Execute` and you will get the result as either **0 (real note)** or **1 (fake note)**.


### Note:
- You can choose the docker image name of your choice when building the docker image (that is in step 2 you can choose another name instead of *bank_api* and use the same name in step 3.)
