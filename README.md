# commentAnalysisSystem
SwearWord Removal and Sentiment analysis of comments on social media for good insight on posts.

(Sentiment LSTM model in this project has been trained on 25000 film reviews of the imdb dataset and has an accuracy of 85.8% in predicting positive(1)/negative(0) respones)

//Load the 'sentiment model.h5' and 'vocabFile.txt' for prediction of sentiments directly(without training model again).
//ie- run cells after 'loadModel and Predicting' only; post importing the above 2 files.

//The LSTM model has been tested for production environment using a single server queuing system with a server traffic of 50 comments/second(youtube traffic).
//The overall model has :  averageDelay = 0.5sec, expectedAverageNumberInQueue = 25, expectedUtilisationOfServer = 0.675
