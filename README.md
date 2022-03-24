#### Counting red blood cells in medical imagery, without deep learning

The field of computer vision has largely come to be associated with deep learning, but this was not always so. There are many classical algorithms and approaches that do not require time and computation-intensive neural networks. The following is one such example. The task was to count the number of red blood cells (RBCs) in a series of images. 

The above was accomplished by utilizing a series of classical computer vision techniques. These include:
- manual and automatic thresholding (Otsu’s algorithm) to binarize the image
- investigating different colour spaces (e.g. HSV), and their individual channels, to find the highest contrast
- low-pass filtering to clean noise
- and finally, flood-fill with labeling (colouring) to count objects (connected-component counting).

The above approach takes a fraction of the time and computation that would have been needed with even a simple deep-learning based approach.

This task was done as part of a university assignment. The main output was a Jupyter notebook with all the code, and a summary report. This report is much shorter than the notebook, and is the recommended starting point if you are new to the domain and wish to explore the problem.

Please note that direct use of OpenCV functions was not allowed, except to open and display the file. All the functions have been coded by hand (e.g. for thresholding, low-pass, flood-fill, connected component counting etc). This made it an excellent learning exercise.
