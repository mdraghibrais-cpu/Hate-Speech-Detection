	1. Applied_ML_Report_Work.ipynb

The notebook was run on Google Colab, the Hate Speech datasets are downloaded through Drive and saved during the current Colab session or the working directory if running it on an IDE.

It requires the installation of prettytable:

  !pip install prettytable



	2. Group_9_Hate_Speech_Models.ipynb

The notebook was run on Google Colab, it installs Keras Tuner and the following nltk packages:

  pip install -q -U keras-tuner

  nltk.download('stopwords')
  nltk.download('averaged_perceptron_tagger')
  nltk.download('punkt')
  nltk.download('wordnet')

The Hate Speech datasets are downloaded through Drive and saved during the current Colab session or the
working directory if running it on an IDE.

The tuning process takes a long time, the recommendation is to skip the code following code chunks:

  - tuner_1.search(train_dataset, epochs = 50, validation_data = val_dataset, callbacks=[stop_early])
  - tuner_2.search(train_dataset, epochs = 50, validation_data = val_dataset, callbacks=[stop_early])
  - tuner_3.search(train_dataset, epochs = 50, validation_data = val_dataset, callbacks=[stop_early]) 