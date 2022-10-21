

Documentation: https://mmdetection.readthedocs.io/

## Introduction

English | [简体中文](README_zh-CN.md)

Run Faster-RCNN-resnet18:
```
python -m torch.distributed.launch --nproc_per_node=8 --master_port='23565' \
    tools/train.py configs/faster_rcnn/faster_rcnn_r18_fpn_1x_coco.py \
    --work-dir /job_data/  \
    --launcher pytorch 
```

Run Faster-RCNN-resnet50:
```
python -m torch.distributed.launch --nproc_per_node=8 --master_port='23565' \
    tools/train.py configs/faster_rcnn/faster_rcnn_r50_fpn_1x_coco.py \
    --work-dir /job_data/  \
    --launcher pytorch 
```

Run Mask-RCNN-resnet18:
```
python -m torch.distributed.launch --nproc_per_node=8 --master_port='23565' \
    tools/train.py configs/mask_rcnn/mask_rcnn_r18_fpn_1x_coco.py \
    --work-dir /job_data/  \
    --launcher pytorch 
```

Run Mask-RCNN-resnet50:
```
python -m torch.distributed.launch --nproc_per_node=8 --master_port='23565' \
    tools/train.py configs/mask_rcnn/mask_rcnn_r50_fpn_1x_coco.py \
    --work-dir /job_data/  \
    --launcher pytorch 
```

Run Cascade-RCNN-resnet50:
```
python -m torch.distributed.launch --nproc_per_node=8 --master_port='23565' \
    tools/train.py configs/cascade_rcnn/cascade_rcnn_r50_fpn_1x_coco.py \
    --work-dir /job_data/  \
    --launcher pytorch 
```

This repo is referred from MMDetection.