# ALTERNATE APPROACH TO MULTILINGUAL SENTIMENTAL ANALYSIS OF TWEETS

This project contains various datasets and Jupyter notebooks for data analysis.

## Directory Structure

The project is organized into the following directories:

- `Code`: This directory contains all the Jupyter notebooks.
- `Datasets`: This directory contains all the original data extracted related to Arvind Kejriwal, Narendra Modi, and Rahul Gandhi.
- `Font`: This directory contains the TrueType font file.
- `SentiWordNet`: This directory contains the Hindi and Telugu SentiWordNet files.
- `Temp`: This directory is used for temporary storage during data processing.

## Files

- `Code/SampleDatasetCreation.ipynb`: This Jupyter notebook contains the code for creating the sample dataset. The output of this code is 'sample_tweets.csv'.
- `Datasets/sample_tweets.csv`: This file contains a sample of tweets generated by 'SampleDatasetCreation.ipynb'.
- `Datasets/labelled_sample_tweets.csv`: This file contains a sample of labelled tweets. The sentiments in 'sample_tweets.csv' are manually labelled to create this file.
- `Code/BaselineMethod.ipynb`: This Jupyter notebook contains the implementation of the baseline method. It uses 'labelled_sample_tweets.csv' as input and creates 'BaseLineApproach_Final_tweets.csv'.
- `Datasets/BaseLineApproach_Final_tweets.csv`: This file contains the final tweets used in the baseline approach, generated by 'BaselineMethod.ipynb'.
- `Code/EmojiBasedMethod.ipynb`: This Jupyter notebook contains the implementation of the emoji-based method. It uses 'BaseLineApproach_Final_tweets.csv' as input.
- `SentiWordNet/HSWN_WN.txt`: This is the Hindi SentiWordNet file.
- `SentiWordNet/TE_AMBI.txt`, `SentiWordNet/TE_NEG.txt`, `SentiWordNet/TE_NEU.txt`, `SentiWordNet/TE_POS.txt`: These are the Telugu SentiWordNet files.
- `Font/Nirmala.ttf`: This is a TrueType font file.

## Workflow

1. Run 'SampleDatasetCreation.ipynb' to generate 'sample_tweets.csv'.
2. Manually label the sentiments in 'sample_tweets.csv' and create 'labelled_sample_tweets.csv'.
3. Run 'BaselineMethod.ipynb' to create 'BaseLineApproach_Final_tweets.csv'.
4. Run 'EmojiBasedMethod.ipynb' which takes in 'BaseLineApproach_Final_tweets.csv'.