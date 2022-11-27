This model will be used for Car color detection(i.e blue,red,beige and so on)
The libraries required to run this model is present in the requirements.txt file


User Manual

To run this model download the conda environment in the machine and then run the following command after changing the directory to yolov5-master:
```python detect.py --weights best.pt --conf 0.25 --source 0  # webcam
			  1 # if the camera is attached in some other port
                          img.jpg  # image 
                          vid.mp4  # video
                          path/  # directory
                          'path/*.jpg'  # glob
                          'https://youtu.be/Zgi9g1ksQHc'  # YouTube
                          'rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP stream
			  ```

```
C:\Users\USER\Desktop\car-color detection\yolov5-master>python detect.py --source blue_car.jpg --weights best.pt

detect: weights=['best.pt'], source=blue_car.jpg, data=data\coco128.yaml, imgsz=[640, 640], conf_thres=0.25, iou_thres=0.45, max_det=1000, device=, view_img=False, save_txt=False, save_conf=False, save_crop=False, nosave=False, classes=None, agnostic_nms=False, augment=False, visualize=False, update=False, project=runs\detect, name=exp, exist_ok=False, line_thickness=3, hide_labels=False, hide_conf=False, half=False, dnn=False, vid_stride=1
C:\Users\USER\AppData\Local\Programs\Python\Python39\lib\site-packages\torch\cuda\__init__.py:83: UserWarning: CUDA initialization: CUDA driver initialization failed, you might not have a CUDA gpu. (Triggered internally at  C:\actions-runner\_work\pytorch\pytorch\builder\windows\pytorch\c10\cuda\CUDAFunctions.cpp:109.)
  return torch._C._cuda_getDeviceCount() > 0
YOLOv5  2022-9-6 Python-3.9.13 torch-1.12.1+cu113 CPU

Fusing layers...
Model summary: 224 layers, 7075486 parameters, 0 gradients
image 1/1 C:\Users\USER\Desktop\car-color detection\yolov5-master\blue_car.jpg: 544x640 1 blue car, 500.0ms
Speed: 0.0ms pre-process, 500.0ms inference, 0.0ms NMS per image at shape (1, 3, 640, 640)
Results saved to runs\detect\exp3
```
