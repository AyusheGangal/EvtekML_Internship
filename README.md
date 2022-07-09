# Patch your Trash
A patch-based implementation of Fully Convoluted Neural Network (FCN) for the detection of soft drink bottles in the trash for easy recycling.

The dataset consists of 200 RGB images, where each image contains 8 containers and is accompanied by a mask which contains a semantic segmentation of the image. The goal is to identify, implement and train a Neural Network architecture which is able to detect each container and output its orientation, spatial boundaries and label. The labels in question are Cola bottle, Fanta bottle, Cherry Coke bottle, Coke Zero bottle, Mtn Dew bottle, Fanta can, Cola can.

In order to efficiently load and process the given data images in the FCNN, I have utilized a patch-based approach. The proposed solution mitigated the GPU usage and used less RAM as well. The proposed solution was able to achieve upto **98.78%** accuracy in predicting the class labels for the test set.

The following steps should be followed to run the proposed 'Patch-your-Trash' system:
1. Download the dataset from the link in the 'Patch-your-Trash/Data.txt'.
2. In order to successfully run the system locally:
    - Install Python3
    - Set the correct path for the dataset by altering the file path in the first cell and in the labels_to_pickle() function in the second cell and setting it to be the location of the dataset in the file explorer/finder.

3. To run the the system in google colab: 
    - Import the downloaded dataset in your drive.
    - Run the cells in the iPython notebook and mount the drive by entering your credentials.
    - set the correct path to the dataset in the drive by altering the file path in the first cell and in the labels_to_pickle() function in the second cell.

