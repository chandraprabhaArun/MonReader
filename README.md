MonReader

MonReader is an innovative mobile document digitization tool designed for the visually impaired, researchers, and those seeking fully automatic, high-speed, and high-quality bulk document scanning. The mobile app simplifies the process—users flip pages, and MonReader handles the rest, detecting flips, capturing high-res images, recognizing corners, cropping, dewarping, and enhancing text contrast. We collected labeled page-flipping videos from smartphones, extracted frames, and aimed to predict page flips from single images.

Data Collection:

Gathered page-flipping videos from smartphones, labeling them as flipping or not flipping.
Trimmed videos into short clips, labeling them accordingly.
Saved extracted frames with a structured naming convention: VideoID_FrameNumber.
Objective:
Predict page flips from single images.

Workflow:

Loaded data into separate training and testing datasets.
Resized and rescaled images for lower-dimensional simplicity.
Created a custom Convolutional Neural Network (CNN) model.
Results:

The model successfully predicted page flips, showcasing its effectiveness in document digitization.

I've started by loading the data into two separate datasets of training and testing. Then, I've resized and rescaled the images for it to be in a lower-dimension which leads to simpler modeling and computation. At last, I've created a custom Convolutional Neural Network (CNN) model and applied it to the data and it yielded the following:

The maximum accuracy on the training data: 0.9983
The maximum accuracy on the testing data: 0.9933
The maximum F1-Score on the training data: 0.9984
The maximum F1-Score on the testing data: 0.9934
