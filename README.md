# Sentiment Analysis - Twitter
Sentiment analysis on tweets was performed to classify tweets as positive, neutral or negative. Implemented on sentiment140 dataset obtained from Kaggle.

### Preprocessing 

1. Run `preprocess.py <raw-csv-path>` on both train and test data. This will generate a preprocessed version of the dataset.
2. Run `stats.py <preprocessed-csv-path>` where `<preprocessed-csv-path>` is the path of csv generated from `preprocess.py`. This gives general statistical information about the dataset and will two pickle files which are the frequency distribution of unigrams and bigrams in the training dataset. 

After the above steps, you should have four files in total: `<preprocessed-train-csv>`, `<preprocessed-test-csv>`, `<freqdist>`, and `<freqdist-bi>` which are preprocessed train dataset, preprocessed test dataset, frequency distribution of unigrams and frequency distribution of bigrams respectively.

For all the methods that follow, change the values of `TRAIN_PROCESSED_FILE`, `TEST_PROCESSED_FILE`, `FREQ_DIST_FILE`, and `BI_FREQ_DIST_FILE` to your own paths in the respective files. Wherever applicable, values of `USE_BIGRAMS` and `FEAT_TYPE` can be changed to obtain results using different types of features as described in report.

### Baseline
 Run `baseline.py`. With `TRAIN = True` it will show the accuracy results on training dataset.

### SVM
 Run `svm.py`. With `TRAIN = True` it will show the accuracy results on 10% validation dataset.

## Information about other files

* `dataset/positive-words.txt`: List of positive words.
* `dataset/negative-words.txt`: List of negative words.


