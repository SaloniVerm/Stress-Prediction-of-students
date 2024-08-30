# Stress-Prediction-of-students
Data link: https://www.kaggle.com/datasets/rxnach/student-stress-factors-a-comprehensive-analysis

# Introduction
The provided dataset contains information regarding student stress factors. Specifically, it contains 20 of them, each of them measured scientifically with the proper scale. All of this information was obtained via surveys.

Our objective will be to reveal how each factor influences the student. Understanding its impact can be meaningful to identify key areas for interventions and psychological support. In order to do this, we will answer the questions provided by the dataset creator.

Before addresing such questions, one would rather do a brief examination of the dataset.
# Breif Examination
So, all columns are the same dtype, and it is numerical! Also, the index represents the number of each student, so we also know there are 1100 students.

20 columns are way too much to use the describe method. Let's use a boxplots in each column to see it visually.
What percentage of students have reported experiencing depression?
Depression levels on this dataset were measured using the Patient Health Questionnaire (PHQ-9). The interpretation of total score provided by this test is:

Total Score	Depression Severity
1-4 - Minimal depression
5-9	 - Mild depression
10-14  -	Moderate depression
15-19  -	Moderately severe depression
20-27	  -Severe depression
Without expertise on this subject, this analysis will consider above "Moderate depression" as "experiencing depression" as, otherwise, the percentage of students who have reported depression would be almost a 100%.
# General Exploration
1) Which factor (Psychological, Physiological, Environmental, Academic, Social) has the highest number of students reporting negative experiences or conditions?

To answer this question, new dataframes, divided by factors, need to be made. Creating these dataframes provides a great opportunity aswell to set the threshold for "negative experience". However, there exists a little challenge added to this. On some columns, higher values is positive (academic performance, safety, living conditions) while on others it is negative (anxiety level, depression, headache).

Also, for later questions, df_categories will be created. This dataframe will divide features on each factor, on their original values.

Selecting those values where depression is higher than 10 and dividing by the total length will deliver the answer to this question.
# Conclusions
On this analysis, all questions asked on the dataset card were answered, aswell as creating a model to predict the anxiety level. As seen on general exploration, correlations exhibit relatively high values, positive or negative, regarding anxiety levels. Therefore, working on improvements on each feature could be used as a mean to achieve improvements on the life of the students. Specifically, bullying and future carreer concerns, being easier to solve on the school side than, say, enviromental factors, should be looked into and dealt with.
