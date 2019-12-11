# Harvard's CS50 Final Project: Argus - Computer Vision (Object Detection)

## Date

3rd December 2019

## Author

n-clarke

## Description

Argus is a computer vision application, which analyses videos and performs object detection on the extracted from the videos frames.

## Used technologies

For demonstration purposes I am using Jupiter labs.

For the project I have made use of a few pre-existing public libraries and resources.
These include Pytorch, TorchVision, Open Cv and Yolo V3 Model Weights.

## Projects contains methods with funcionalities:

- delete_folder_contents(folder_url): Deleting existing files from folders - purely for clean-up.

- detect_objects(model, img): Detecting objects - this evaluates an image and return the number of detected objects.

- show_objects(img, detections, image_name): Showing objects - used to draw the bounding boxes around detected objects (rectangles), and then save the processed images.

- analyse_images(source): Analysing images - this function iterates through all the images from a specific directory and processes them.

- convert_video_into_frames(video_src, save_to_folder_path): Splitting video into frames and saving them as images.

- create_video(image_folder_src, video_name, fps): Creating a video from all processed images from a specified directory.

- run(video_name, file_type): Enter the video name and extension to be processed.

For the purpose of this project, all above functions are used in combination,
in order to obtain final video consisting of processed video frames with drawn detections and detected objects classes.

## Pre-Requistes

Download and install Anaconda for your OS

```
https://docs.anaconda.com/anaconda/install/
```

Download the project to your machine
```
/workspace/project/object-detection
```
Delete the followling files from the project source code
```
object-detection/data/object_detection/README.md
object-detection/data/object_detection_processed/README.md
object-detection/data/object_detection_video/README.md
```

## To Run

1) Open Anaconda Navigator.

2) Then Open Jupyter Notebooks.

3) If successful Jupter Notebooks should load on http://localhost:8888/tree
```
Note the port :8888 maybe different
```
4) Navigation using the file directory and open object-detection-project.ipynb

5) Wait until the kernel has loaded. If prompted use Python 3.

6) Go to data/object_detection_video/ an save the video you wish to be processed for object detection.

7) On Execute Program in the object-detection-project.ipynb on the last cell change the following
```
run('street_bike', '.mp4')

to

run('YOUR_VIDEO_NAME', 'YOUR_VIDEO_FORMAT')

Where:
    YOUR_VIDEO_NAME = your video name
    YOUR_VIDEO_FORMAT = your video format (e.g. .mp4, .avi, .mov)
```

7) Click Kernel > Restart and Run All.

or

7) Click manually on each cell and run.

8) The program has now successfully be executed.

## Output

To view and get your processed video go to
'''
Path:
data/object_detection_video/

Your new file will be formatted as:
{FileName}_processed_od
'''
