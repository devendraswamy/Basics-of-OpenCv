# Basics-of-OpenCv
Here I post the all the basics and important codes related the OpenCV

Here I can Kept all the codes from Begging to advance level of opencv  

Here I mentioned deatails about Load_iamge_opencv.py

OpenCV load image (cv2.imread)
In the first part of this tutorial, we’ll discuss how to load an image from disk using OpenCV and the cv2.imread function.

From there, you’ll learn how to configure your development environment to install OpenCV.

We will then review our project directory structure, followed by implementing load_image_opencv.py, a Python script that will load input images from disk using OpenCV and the cv2.imread function.

We’ll wrap up this tutorial with a discussion of our results.

Here I am purposely providing an image path that does not exist on my disk.

When I pass an invalid image path to OpenCV’s cv2.imread function, cv2.imread returns None.

And when I try to grab the image width, height, and number of channels, Python errors out with an AttributeError, saying that the NoneType object does not have a shape attribute.

This error makes sense when you think about it:

If you supply an invalid image path to cv2.imread, the function will return None.
However, our code assumes the image path is correct and thus returns a NumPy array.
But if the returned image is None, then it is not a valid NumPy array, hence the error.
