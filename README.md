# Introduction

This app uses convolutional neural networks to classify seismogram data into a positive and negative class. Two competing objectives dictate the model design: (1) reducing the number of false positives and (2) doing early on detection. Hidden Markov Models are considered as an alternative. 

# Data Processing

- Fixed sizes of arrays
- Created conditionals to ensure size of time array is consistent 

# Feature Selection

- Used TSFresh to extract features
    - x, y and z abs_energy
    - x, y and z mean 
    - x, y and z median
    - x, y and z sum_values
    - x, y and z maximum
- For future work, I could consider using a 2DFFT spectrum as a feature

# Model Selection

TBD

# Prediction and Results

TBD

# Future Work
- Finish getting CNN to work 
- Get confusion matrix and accuracy number
- Re-do trainig and validation with smaller windows of data. Check minimum window for high accuracy.
- Do classification for every 4s window, check how early we can detect an earthquake.
- Re-do training with some information about how much more often 'noise' files exist than 'earthquake' file, instead of assuming they are equally likely events
- Make unit test cases
- Get `requirements.txt` and make Travis integration tests
