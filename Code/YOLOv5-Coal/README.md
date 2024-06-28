# YOLOv5-Coal

## Requirements

```
pip install -r requirements.txt  # install
```

## Train 

```
python train.py --data Coal.yaml --cfg yolov5n-Coal.yaml --weights yolov5n.pt --hyp hyp.coal.yaml --img 640 --workers 15 --device 0 --patience 50 --batch-size 32 --epochs 300 
```

## Test

```
python val.py --data Coal.yaml --weights ./runs/train/exp/weights/best.pt --img 640 --batch 32 --device 0 --task test --save-json
```
