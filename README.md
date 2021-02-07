# ABOUT RECOGNITO
Recognito is a handwritten digit recognition system that uses convolutional neural networks to predict manual handwritten data. It uses different python libraries and the MNIST database for its training.The project recognito won the best project award in the annual expertshub internship 2018.
# PROBLEM STATEMENT
Given a set of manually written data, the software should be able to predict the data based on its learning and most accurately output the handwritten data.
# APPROACH
This was a very interesting and a simple problem. We fetched the training and testing datasets from the MNIST database and trained our model to recognize a large variety of handwritings.
# ABOUT MNIST DATABASE
Developing such a system includes a machine to understand and classify the images of handwritten digits as 10 digits (0–9). Samples provided from MNIST (Modified National Institute of Standards and Technology) dataset includes handwritten digits total of 70,000 images consisting of 60,000 examples in training set and 10,000 examples in testing set, both with labeled images from 10 digits (0 to 9). This is a small segment form the wide set from NIST where size was normalized to fit a 20*20 pixel box and not altering the aspect ratio. Handwritten digits are images in the form of 28*28 gray scale intensities of images representing an image along with the first column to be a label (0 to 9) for every image. The same has opted for the case of the testing set as 10,000 images with a label of 0 to 9.
# AVAILABLE FILES IN THE DATASET
So, before starting further deep in this topic, the better point should be to get familiar with the provided dataset. Following points are same in training and testing set along with the set of the images and labels files –
1. Pixels are arranged row-wise, ranging from 0 to 255, as from RGB color code.
2. Background as white (0 value from RGB) and foreground as black (255 value from RGB).
3. Labels of digits classified from 0 to 9.

There are four files of training and testing are:
1. Training set images files 
2. Training set labels file 
3. Test set images files 
4. Test set label files 

# ALGORITHM
We used the concept of a convolutional neural network system to design this software.
To see the performing steps for a system to predict, we can define algorithms as –
1. Break the image into small image tiles — Similar to sliding window, we can pass sliding window over the entire large image and each result is saved as separate, as a segment of large image as tiny picture tile.
2. Feeding each tiny tile into the smaller size neural network — we rarely initialize the parameters with the same values and if not so, then we mark that tile as interesting.
3. Save the results from each small tile into a new array — we would not like to misplace the index of the original file. So we place the results in a grid of the same arrangement as an original image.
4.Downsampling — to reduce the size of a newer array, downsampling is used by max-pooling.
