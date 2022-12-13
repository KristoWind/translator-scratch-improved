# translator-scratch-improved
Transformer translator (eng-nld) from scratch. Improved version of François Chollet's 'Deep Learning with Python' Transformer from chapter 11. The code of François Chollet's Transformer model can be found on https://colab.research.google.com/github/fchollet/deep-learning-with-python-notebooks/blob/master/chapter11_part04_sequence-to-sequence-learning.ipynb

# The change
Chollet uses the RMSProp optimizer in his code (2021). Using the Adam optimization algorithm may help the model converge faster and potentially achieve better performance than using the default optimizer. Adam combines the advantages of both SGD and RMSProp, and can adaptively adjust the learning rates of different parameters in the model based on the historical gradient information. This can help the model avoid getting stuck in suboptimal solutions and improve its convergence.

Chollet's model achieves a test accuracy of 0.8811 with the RMSProp optimizer on 30 epochs. My improved model scores a test accuracy of 0.8953 using the Adam optimizer on 20 epochs.
