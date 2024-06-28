# YOLOv10-Coal

## Requirements

```
pip install -r requirements.txt
```

## Train

```
# yolov10n-Coal
yolo detect train data=Coal.yaml model=yolov10n-Coal.yaml pretrained=yolov10n.pt epochs=300 imgsz=640 workers=15 batch=32 optimizer='SGD' lr0=0.01 lrf=0.01 momentum=0.937 weight_decay=0.0005 patience=50

# yolov10s-Coal
yolo detect train data=Coal.yaml model=yolov10s-Coal.yaml pretrained=yolov10s.pt epochs=300 imgsz=640 workers=15 batch=32 optimizer='SGD' lr0=0.01 lrf=0.01 momentum=0.937 weight_decay=0.0005 patience=50
```

## Test

```
yolo val data=Coal.yaml model=./runs/detect/train/weights/best.pt split=test save_json=True
```
