Sleep_Stage_Classification

Project description:
In this project, we set out to predict which sleep stage a patient is in using physiological signals collected during sleep. We framed the task as a classification problem, where segments of sleep data were mapped to standard sleep stages such as Wake, light sleep, deep sleep, and REM. After preprocessing and cleaning the data, we trained and compared multiple models, including a convolutional neural network (CNN) and several multilayer perceptron (MLP) variants using different activation functions, to capture patterns in the signals. The models were evaluated using standard classification metrics to compare their performance across the different sleep stages.

Steps:

1. Import requirements in requirements.txt file
- pip3 install -r requirements.txt
2. If you want to download any of the edf files labeled SNXXX, use the following curl commands:
  curl -L -o SN002.edf "https://physionet.org/files/hmc-sleep-staging/1.1/recordings/SN002.edf?download"
  curl -L -o SN002_sleepscoring.edf "https://physionet.org/files/hmc-sleep-staclearging/1.1/recordings/SN002_sleepscoring.edf?download". Or, you can also use the download.py file,
  modify the bounds of the "for i in range" loop, and it will retrieve and download the corresponding edf files for those recordings.
  - Right now, the project uses SN001, SN002, SN003 to train the model and SN005 to test, but we will have to use more to train it fully.
