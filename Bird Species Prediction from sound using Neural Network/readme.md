## Summary

This report focuses on developing neural network models for bird species classification based on audio spectrograms. The key aspects covered are:

**Data Preprocessing**:
- The dataset contains spectrograms of 10 audio clips for 12 bird species, along with 3 unlabeled clips for testing.
- For binary classification, features and labels were extracted for the 'daejun' and 'houfin' species.
- For multiclass classification, features were extracted for all 12 species.
- Unlabeled data was preprocessed using librosa to compute mel-spectrograms from audio files.

**Binary Classification**:
- A Convolutional Neural Network (CNN) with dropout and a simple Neural Network (NN) were developed.
- The CNN achieved 100% training accuracy and 100% test accuracy with low training (0.0024) and test loss (0.007).
- The simple NN achieved 100% training accuracy and 95% test accuracy with training loss of 0.0011 and test loss of 0.077.

**Multiclass Classification**:
- Three models were developed: CNN, CNN with dropout, and simple NN.
- The CNN with dropout performed best with 97.22% training accuracy, 71.55% test accuracy, training loss of 0.0806, and test loss of 2.10.[1]
- The basic CNN had 99.62% training accuracy but lower 66.37% test accuracy, indicating overfitting.
- The simple NN underperformed with 60.81% training accuracy and 56% test accuracy.

**Testing on Unlabeled Data**:
- The CNN with dropout model was used to predict species for 3 unlabeled audio clips.
- For each clip, the top 3 predicted species with their probabilities are reported.

The report highlights the effectiveness of CNNs, especially with dropout regularization, in classifying bird species from audio data. It also emphasizes the importance of appropriate model selection and regularization techniques to prevent overfitting.


