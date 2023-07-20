# Lane Detection in Videos and Images using OpenCV

This Jupyter notebook contains code for lane detection in videos and Images using OpenCV library. The code uses the Hough Transform
algorithm to detect lines in the video frames, and then averages out these lines to get the final lane lines. The final
lane lines are then drawn on the original video frames.

## Installation

To run this notebook, you need to have the following libraries installed:

- OpenCV
- NumPy
- Matplotlib

You can install these libraries using pip:

```
pip install opencv-python
pip install numpy
pip install matplotlib
```

## Usage

To use this code, you need to have a video file that contains the footage of a road. The code expects the video file to
be in the same directory as this notebook. You should also change the `video_name` variable to the name of your video
file.

Once you have made these changes, you can run the code. The code will read the video file, detect the lanes in each
frame, and write the output video to a file called `output_vid_1.mp4` (or `output_vid_2.mp4` for video 2).

## Code Overview

The code can be divided into the following parts:

1. Reading the input video file and setting up the output video file.
2. Applying CLAHE filter for haze conditions (only for video 2).
3. Detecting lanes in each frame using Hough Transform algorithm.
4. Averaging out the detected lines to get the final lane lines.
5. Drawing the final lane lines on the original video frames.
6. Writing the output video to file.

## Results

The code works well for detecting lanes in videos. The output video shows the detected lanes overlayed on the original
video frames. The results can be further improved by tweaking the parameters of the Hough Transform algorithm and the
region of interest mask.

## Conclusion

In conclusion, this Jupyter notebook provides a simple and effective solution for detecting lanes in videos using OpenCV
library. It can be used for a variety of applications such as self-driving cars, lane departure warning systems, and
more.