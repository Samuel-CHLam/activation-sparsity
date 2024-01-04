# Deep Neural Network Initialization with Sparsity Inducing Activations
Submitted to ICLR 2024 (awaiting final decision), accepted in CPAL 2024 (Poster, non-archival spotlight track). Will be available on arXiv soon.

- CPAL 2024 Poster
- [Latest version of conference paper (ICLR 2024 OpenReview page)](https://openreview.net/forum?id=uvXK8Xk9Jk&noteId=DY1IL28Qdu)
- [CPAL version of conference paper (CPAL 2024 OpenReview page)](https://openreview.net/forum?id=QV5qqLfcYy)

## Abstract
Inducing and leveraging sparse activations during training and inference is a promising avenue for improving the computational efficiency of deep networks, which is increasingly important as network sizes continue to grow and their application becomes more widespread.  Here we use the large width Gaussian process limit to analyze the behaviour, at random initialization, of nonlinear activations that induce sparsity in the hidden outputs.  A previously unreported form of training instability is proven for arguably two of the most natural candidates for hidden layer sparsification; those being a shifted ReLU ($\phi(x)=\max(0, x-\tau)$ for $\tau\ge 0$) and soft thresholding ($\phi(x)=0$ for $|x|\le\tau$ and $x-\text{sign}(x)\tau$ for $|x|>\tau$).  We show that this instability is overcome by clipping the nonlinear activation magnitude, at a level prescribed by the shape of the associated Gaussian process variance map. Numerical experiments verify the theory and show that the proposed magnitude clipped sparsifying activations can be trained with training and test fractional sparsity as high as 85\% while retaining close to full accuracy.
