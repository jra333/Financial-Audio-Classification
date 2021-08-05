![Banner](https://i.gyazo.com/2e52e69c80f4884d0d3c5e37742115f3.jpg)
# Financial Audio Sentiment Classification and Analysis

We aim to solve the lack of audio analysis within the financial industry, more notably market sentiment. Using natural language processing (NLP), many analysts usually generate their reports from a textual input (ex. News articles, Twitter tweets etc.) and now with the use of “transformers” these analyses can be very powerful in understanding market volatility and momentum. However, one can argue that traditional sentiment analysis can sometimes lack in depth, as written language can be highly subjective, not being able to fully capture the many facets that contribute to an individual's true expression that which we mark as sentiment. By classifying audio segments in conjunction with NLP generated sentiment, predictability of our three distinct classes ("bullish", "bearish" and "neutral") increases exponentially. 

Our data was self-ensembled and extracted from over 11,0000 YouTube videos and, from them we extract audio specific features. Further, because these YouTube videos contained over 130,000 useful sentence segements (utterances) annotating each audio individually would be a tedious task. To remedy this, we implemented an automated method that makes use of Googles BERT transformer. From the audio speech to text transcription + annotation, we then performed a series of steps that created audio sentence/phrase segments paired with its respective class. The final training/validation dataset after augmentations resulted in more than 300,000 "bullish", "bearish" and "neutral" audio signals and mel-spectrograms. 

We trained our data on four baseline models:
- Logistic Regression
- Support Vector Classifier (SVC) x2
- XGBoost

And a few neural netowrks for deep learning:
- Tested: ResNet50, VGG16, EfficientNetB0 and B7
- Tested: 4 unique architectures from scratch

### Table of Contents:
- **Approach**
    - Notebooks:
        - [Ensembling](https://github.com/jra333/Financial-Audio-Classification/blob/main/Dataset%20Ensembling/dataset_ensembling.ipynb)
        - [EDA](https://github.com/jra333/Financial-Audio-Classification/blob/main/EDA%20_Augmentations/exploratory_data_analysis.ipynb)
          - [Augmentations](https://github.com/jra333/Financial-Audio-Classification/blob/main/EDA%20_Augmentations/datasetsplit_augmentations.ipynb)
        - [Baseline Models](https://github.com/jra333/Financial-Audio-Classification/blob/main/Baseline%20Modeling/features_baseline_modeling.ipynb)
        - [Deep Learning](https://github.com/jra333/Financial-Audio-Classification/blob/main/Ext.%20Modeling%20(Deep%20Learning)/extended_modeling(deep%20learning).ipynb)
- **Findings**
    - [Report]
- [**Future Work**](https://github.com/jra333/Financial-Audio-Classification#future-work)


## Results


## Future Work

This project is ongoing. Current focus is:

- Restructure ensembled data (possibly collect more)
- Revise augmentations
- Improve CNN accuracy 
- Clean model pipelines and dataloading flow


For a more detailed explanation, read the report here: 


