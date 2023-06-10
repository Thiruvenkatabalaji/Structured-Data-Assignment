# Structured-Data-Assignment


Data Description -
The folder shared with you contains following four files
1) Train.parquet - Dataset to be used for training
2) Test.parquet - Dataset to be used for testing
3) Sample_submission.csv - a sample csv file showing how the output should be
4) Final_submission.csv - csv file to be submitted finally after generating the output
Brief Description of the Dataset -
The dataset in question contains a comprehensive collection of electronic
health records belonging to patients who have been diagnosed with a specific
disease. These health records comprise a detailed log of every aspect of the
patients' medical history, including all diagnoses, symptoms, prescribed drug
treatments, and medical tests that they have undergone. Each row represents a
healthcare record/medical event for a patient and it includes a timestamp for each
entry/event, thereby allowing for a chronological view of the patient's medical history
The Data has mainly three columns
1) Patient-Uid - Unique Alphanumeric Identifier for a patient
2) Date - Date when patient encountered the event.
3) Incident - This columns describes which event occurred on the day.


Problem Statement
Problem 1 - The development of drugs is critical in providing therapeutic options
for patients suffering from chronic and terminal illnesses. “Target Drug”, in particular,
is designed to enhance the patient's health and well-being without causing
dependence on other medications that could potentially lead to severe and
life-threatening side effects. These drugs are specifically tailored to treat a particular
disease or condition, offering a more focused and effective approach to treatment,
while minimising the risk of harmful reactions.
The objective in this assignment is to develop a predictive model which will predict
whether a patient will be eligible*** for “Target Drug” or not in next 30 days. Knowing
if the patient is eligible or not will help physician treating the patient make informed
decision on the which treatments to give.
*** - A patient is considered eligible for a particular drug when they have taken their
first prescription for that drug. Below table gives an example



Please follow below steps for developing the model -
A. Come up with a positive and negative set for developing the model, here the positive
point is the patient who has taken ‘Target Drug”. Make sure you are also taking into
account the time aspect while coming up with a positive & negative set because the
aim is to predict 30 days in advance whether a patient is going to be eligible or not.
B. Come up with the right kind of feature engineering for developing your model. The
features can be frequency-based, time-based etc. If possible can also leverage deep
learning techniques
C. Evaluate the model on validation set & come up with the right strategy to reduce false
positives & false negatives.
D. Once you have developed your predictive model, use your model to generate
predictions for patients in test.parquet, each patient in test.parquet should be labelled
as 1 or 0 using your predictive model and the final generated predictions should be
submitted in final_submission.csv
E. The evaluation metric for the assignment is F1-Score(candidates with the highest
F1 score would be prioritised)
