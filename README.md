# Facial Key Features

This project will be all about defining and training a convolutional neural network to perform facial keypoint detection, and using computer vision techniques to transform images of faces. The project is in partial fullfilment of Udacity's Nanodegree in Computer Vision. 

## Files
This project consists of the following files:

- `1. Load and Visualize Data` Jupyter notebook 
    - Contains the necessary code to load as well as visualize the dataset. This set of image data has been extracted from the YouTube Faces Dataset, which includes videos of people in YouTube videos. These videos have been fed through some processing steps and turned into sets of image frames containing one face and the associated keypoints.
- `2. Define the Network Architecture` Jupyter notebook
    - Contains the details on the architecture of the network used in the project. In this notebook and in `models.py`: 
        - Define a CNN with images as input and keypoints as output
        - Construct the transformed FaceKeypointsDataset, just as before
        - Train the CNN on the training data, tracking loss 
        - See how the trained model performs on test data 
        - If necessary, modify the CNN structure and model hyperparameters, so that it performs well.
- `3. Facial Keypoint Detection, Complete Pipeline` Jupyter notebook
    - After training rained a neural network to detect facial keypoints, you can then apply this network to *any* image that includes faces. The neural network expects a Tensor of a certain size as input and, so, to detect any face, you'll first have to do some pre-processing.
        - Detect all the faces in an image using a face detector (we'll be using a Haar Cascade detector in this notebook).
        - Pre-process those face images so that they are grayscale, and transformed to a Tensor of the input size that your net expects. 
        - Use your trained model to detect facial keypoints on the image.
- `4. Fun with Keypoints` Jupyter notebook
- `5. Zip Your Project Files and Submit` Jupyter notebook
- images folder 
    - contains the images that I will be using in the notebooks

## Notes
The results obtained from this project can still be improved. For instance, I noticed that the Haar Cascade used in detecting faces fails to detect other facial orientations. Best to explore other detectors such as the mtcnn etc. Second, more layers can be added to actually see its effect in improving the loss. 