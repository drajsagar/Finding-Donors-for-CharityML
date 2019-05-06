# Finding-Donors-for-CharityML
Project using supervised learningn to identify potential donors

## Intro 
CharityML is a fictitious charity organization located in the heart of Silicon Valley that was established to provide financial support for people eager to learn machine learning. After nearly 32,000 letters were sent to people in the community, CharityML determined that every donation they received came from someone that was making more than $50,000 annually. To expand their potential donor base, CharityML has decided to send letters to residents of California, but to only those most likely to donate to the charity. With nearly 15 million working Californians, CharityML has brought you on board to help build an algorithm to best identify potential donors and reduce overhead cost of sending mail. Your goal will be evaluate and optimize several different supervised learners to determine which algorithm will provide the highest donation yield while also reducing the total number of letters being sent. 

## Software and Libraries

This project uses the following software and Python libraries:

    Python
    NumPy
    pandas
    scikit-learn (v0.17)
    Matplotlib

## File description


    finding_donors.ipynb: This is the main file where we will be performing the work on the project.
    census.csv: The project dataset. This will be load in the notebook.
    visuals.py: This Python script provides supplementary visualizations for the project.

## Supervised Learning Models
In this project I am going to use the following ML algorthims also, I tried providing some real world applications that these algorthims are used in 

### RandomForest:

RandomForest can be used for both classification, regression as these are ensemble learning methods. RandomForest model is used widely in banking sector to identify the loyal and fraud customers

The strengths of this model are unlike decision trees this model will not over-fit and it can be useful in feature engineering; when the data size is large

RandomForest models need more data; they do not fit elaborate and highly detailed things well when the sample size is low

As said in the example this model can be a right fit to identify particular output in the end, the data set is here is large and there are multiple features available based on which we can come up with a good results

#### Gradient Boosting:

Gradient boosting can be used in the field of learning to rank. The commercial web search engines Yahoo and Yandex use variants of gradient boosting in their machine-learned ranking engines.

This model helps to convert weak learners to strong ones, this helps in achiving the hypothesis by boosting the weak learners quickly

This can overfit if run for too many iterations and sensitive to noisy data and outliers, if we don't tune the parameters the algorithm may fail in achieving the good results

The data we are processing now have less or no outliers also we can tune the data to right fit to achieve better results

### LogisticRegression:

LogisticRegression can be useful to identify the attrition vs retention in operations and win vs loss in games. The data set which we have chosen to work on have good line of separation which I believe a great benefit to achieve good result

As per my findings this model is the best algorithm for predicting probabilities of an event, fast to train and easy to train on big data

In order to fit this models non linear functions a great amount of work is needed. Data we are processing here is well processed and I believe there is not much of changes needed

As were looking for potential donors I believe this can help us predicting the required output list

After looking at the results with training data set I would like to us the Gradient Boosting Classifier algoritham

## Results:

Metric          Unoptimized Model       Optimized Model

Accuracy Score 	0.8630 	             0.8718

F-score 	    0.7395 	             0.7545

The scores of optimized model are better than the unoptimized model And comparing the optimized results with the benchmark results, the acquired result from optimized model are very good

