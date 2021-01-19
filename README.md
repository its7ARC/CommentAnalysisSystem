# Comment Analysis System
Model for Sentiment analysis and filtering of offensive comments on social media.

Sentiment analysis has been performed using a # LSTM model. This model has been trained and tested on 25000 film reviews each of the imdb dataset and has an accuracy of 83.18% for prediction of positive(1)/negative(0) comments.


The LSTM model has been tested for production environment using a Single server queuing system with a server traffic of 50 comments/second(equal to youtube).   
The model has
- Average Delay = 0.5sec
- Expected Average Number in Queue = 25
- Expected Utilisation Of Server = 0.675

Usage instructions-
- Load the 'sentiment model.h5' and 'vocabFile.txt' for prediction of sentiments directly (Without training model again)
- Run cells after 'Overall Model Deployment' in https://github.com/its7ARC/commentAnalysisSystem/blob/master/commentAnalysis.ipynb; 
- Comments shall be entered into the system by appnending comments to corpus in 'In27'. 

Model Output: 
- 'In29' 
- 1-> Positive, 0-> Negative
- Filtered comments do not pass through the model.

Dataset: https://www.kaggle.com/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews

Detailed Project Report: https://github.com/its7ARC/commentAnalysisSystem/blob/master/Comment%20Analysis%20System.pdf
