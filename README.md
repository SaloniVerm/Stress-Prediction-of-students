# Stress-Prediction-of-students
Data link: https://www.kaggle.com/datasets/rxnach/student-stress-factors-a-comprehensive-analysis

# Introduction
The provided dataset contains information regarding student stress factors. Specifically, it contains 20 of them, each of them measured scientifically with the proper scale. All of this information was obtained via surveys.

Our objective will be to reveal how each factor influences the student. Understanding its impact can be meaningful to identify key areas for interventions and psychological support. In order to do this, we will answer the questions provided by the dataset creator.

Before addresing such questions, one would rather do a brief examination of the dataset.
# Breif Examine
So, all columns are the same dtype, and it is numerical! Also, the index represents the number of each student, so we also know there are 1100 students.

20 columns are way too much to use the describe method. Let's use a boxplots in each column to see it visually.
