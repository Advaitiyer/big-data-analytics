## Character Recognition: Can Machine Learning Identify Human Written Characters?

Despite the rise of personal computers and smartphones, many people and businesses are dependant on hand written notes. For many people, written notes are faster and provide better information retention. Despite their benefits, handwritten notes fail to take advantage of modern technology. Drawbacks include inability for easy backup, sharing, and searching among other things. Currently the most popular method for sharing and backing up hand written documents involve photographing or scanning the document and converting it to an image. Now the document is shareable and easily duplicated, however, it still lacks the ability to be searched or understood by a machine. The ability for the document content to be understood by the machine provides numerous benefits including increased accessibility and searchability. We chose to tackle this problem using machine learning methods to attempt to identify individual characters from a 28x28 pixel digital image. 

**Data Description:**

The dataset contains 814,255 observations out of which 558,345 was used for training, 139,587 used for validation, and 116,323 for training. Each observation is a flattened 28 x 28 pixel grayscale image yielding 784 features. Each feature is a pixel grayscale value from 0 (white) to 255 (black). The distribution of characters was not even, with some values like '1' being very common with around 38,000 observations and other values like 'j' less common with around 1,800 observations. 

**Conclusion:**

Handwriting recognition is difficult for both humans and machines. Letters look similar depending on individual’s writing style, and identifying the intricate relations between specific pixel-patterns, and predicting the label correctly is difficult due to very tightly bound decision-boundaries.

The random forest classifier provided 41% accuracy. It was noticeable that deeper trees provided better accuracy, however it was very complex due to the size of the data.

The multi-layer perceptron worked quite well, with the best accuracy at 61%. Increasing the number of hidden layers caused a decrease in the accuracy, most likely because increasing the number of hidden layers from 5 to 10 caused the model to overfit the training data. 

Through PCA, it was concluded that 184 principal components explain more than XX% of the variance, which means, the dimensions of the images can be reduced from 784 to 184, without losing too much information.

It can be speculated that Convolutional Neural Networks (CNNs) might perform better than the multi-layer perceptron.

**Poster with results:**

<img src="https://github.com/Advaitiyer/advaitiyer.github.io/blob/master/assets/images/big-data-analytics/bda-project-poster.pdf?raw=true"/>
