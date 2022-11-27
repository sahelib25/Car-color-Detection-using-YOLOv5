This model will be used for vehicle detection(i.e bus,car or truck)
The libraries required to run this model is present in the requirements.txt file


User Manual

To run this model download the conda environment in the machine and then run the following command after changing the directory to yolov5-master:
python detect.py --weights best.pt --conf 0.25 --source 0  # webcam
			  1 # if the camera is attached in some other port
                          img.jpg  # image 
                          vid.mp4  # video
                          path/  # directory
                          'path/*.jpg'  # glob
                          'https://youtu.be/Zgi9g1ksQHc'  # YouTube
                          'rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP stream