# homework-neural-net

## Background

This is a homework studying neural network using TensorFlow at Google Colab.

The specific apps we use is keras Sequential model over Dense layers.

## Summary

Upon a provided data in csv format: [applicants_data.csv](Resources/applicants_data.csv), we apply the Tensorflow neural network algorithms.

First we analyze, encode and scale the columns. Build feature dataframe X and binary classification labels y.

We then seperate the available X and y into training and test sets.

We then tried different types of models, and pick 3 of them to present in the python jupyter notebook.

We finally save the 3 models in 3 files [AlphabetSoup.h5](AlphabetSoup.h5), [AlphabetSoup A1.h5](AlphabetSoup_A1.h5) and [AlphabetSoup A2.h5](AlphabetSoup_A2.h5).

## Explaination

This data has 116 features when all the string columns get categorically encoded. There are only 3 numeric columns. Although some categorical features appear imbalanced, there is no obvious hint that we can drop any outlier. Except a "classification" column appears containing some rarer occurrences - once only in the data. We tried to model without these columns, no improvement is observed.

## Conclusion

The data passes through the neural net quite consistently, regardless the number of layers, number of perceptrons, or activation methods. We always stop at loss 0.69 and accuracy 0.53, within 15 epochs of training. 

The evaluation over pre-saved test sets are also identical, except the trimmed data having much larger loss figure, but still identical accuracy rate.