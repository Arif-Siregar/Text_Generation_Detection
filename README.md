# Project description
The goal of the project is to correctly identify whether a passage is human written or machine generated. Our approach involves the combination of random forest, SVM and perecptron. For the baseline, we only use the data generated by machine to calculate the probability of each word appearning after a certain word, as machine generated passages tend to be more predicatable than human written.

# Dataset
There are two training datasets: one coming from domain1, and another from domain2 in data repository, each contains both machine-generated and human-authored samples.
The training data is given in newline delimited JSON format, such that each line contains an instance and each instance is a dictionary with keys:
  * text: the sequence of words, after light preprocessing, where each word has been mapped to an index in {0, . . . , 83582}
  * label: a binary label where 0 represents machine-generated data and 1 represents human-generated.

Two files are provided:
  * domain1.json: 5,000 samples (2,500 of each class).
  * domain2.json: 13,000 samples (1,500 human-generated samples, 11,500 AI-generated samples)

# Team 70
Meet the team:  
    * Arifyunanda Siregar bin Suparman
    * Shourya Thapliya
    * Zofia Witkowski-Blake
