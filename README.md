![Banner](https://i.gyazo.com/2e52e69c80f4884d0d3c5e37742115f3.jpg)
# Audio Sentiment Analysis and Classification within the Financial Domain 

From our compiled audio files we aim to solve the lack of audio analysis surrounding the financial industry, more notably market sentiment. Traditional sentiment analysis usually utilizes Natural Language Processing (NLP) but using only text can sometimes lack depth and practicality regarding its interpretability. NLP alone tends to disregard the many facets that contribute to an indivduals sentiment. By classifying audio segments in conjunction with NLP sentiment, predictability of our three distinct classes ("bullish", "bearish" and "neutral") increases exponentially. Our data was self-ensembled and extracted from over 11,0000 YouTube videos and from them we extract audio specific features. Further, because these YouTube videos contained over 130,000 useful sentence segements (utterances) annotating each audio individually would be a tedious task. To remedy this, we implemented an automated method that makes use of Googles BERT transformer. From the audio speech to text transcription + annotation, we then performed a series of steps that created audio sentence/phrase segments paired with its respective class. The final training/validation dataset after augmentations resulted in more than 300,000 "bullish", "bearish" and "neutral" audio signals each containing a mel-spectrogram. 

We trained our data on four baseline models:
- Logistic Regression
- Support Vector Classifier (SVC) x2
- XGBoost

And two neural netowrks for deep learning:
- Custom CNN
- HyperResNet

For a more detailed explanation, read the report here: 


