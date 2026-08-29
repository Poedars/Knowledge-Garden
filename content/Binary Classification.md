In a binary classification problem, the result is a discrete value output.
For example:
- account hacked (1) or not hacked (0)
- a tumor malign (1)or benign(0)

Example: Cat vs Non-Cat
The goal is to train a classifier for which the input is an image represented by a feature vector, 𝑥, and predicts whether thecorresponding label𝑦is 1 or 0. In this case, whether this is a cat image(1)or a non-cat image.
![[Pasted image 20260829162304.png]]

An image is stored in the computer in three separate matrices corresponding to the Red, Green, and Blue color channels of the image. The three matrices have the same size as the image, for example, the resolutionof the cat image is 64 pixels X 64 pixels, the three matrices (RGB) are 64 X 64 each.

The value in a cell represents the pixel intensity which will be used to create a feature vector of n-dimension. In pattern recognition and machine learning, a feature vector represents an image, Then the classifier's job is to determine whether it contain a picture of a cat or not.

To create a feature vector, 𝑥, the pixel intensity values will be “ unrolled” or “ reshaped” for each color. The dimension of the input feature vector𝑥 is𝑛 = 64𝑥 64𝑥 3 = 12288.

more information