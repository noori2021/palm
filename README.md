# MOPAD

These codes and datsets are from the paper "Growing status observation for oil palm tree using Unmanned Aerial Vehicle (UAV) images", which is published in ISPRS Photogrammetry and Remote Sensing.

## Training

```bash
CUDA_VISIBLE_DEVICES=gpu_id python tools/train.py configs/oilPalmUav/mopad.py
```


## Inference for the whole image

```bash
CUDA_VISIBLE_DEVICES=gpu_id python demo/demoFull.py configs/oilPalmUav/mopad.py work_dirs/mopad/latest.pth mopad-det.txt test_images
```

## Models

Our training models for Site 2 can be downloaded from

[Baidu Wangpan](https://pan.baidu.com/s/1Vj-Se2LUi8839_JjYIh2tQ) Access: 7n61

Our training models for Site 1 can be downloaded from

[Baidu Wangpan](https://pan.baidu.com/s/1asWfKmzViQKDRRZ0BPBOXw) Access: 8mwa


## Dataset
Our dataset for Site 2 can be downloaded from

[Google Drive](https://drive.google.com/drive/folders/17I8HVrGo812vpMdD2EKrkdw_61NVrUfb?usp=sharing)

[Baidu Wangpan](https://pan.baidu.com/s/1JStM5aYCjtZho249PuJ_WQ)  Access: qpaw

Our dataset for Site 1 can be downloaded from

[Baidu Wangpan](https://pan.baidu.com/s/1Eyk1fldzNehEOcd6E9UEsw) Access: fgfv

The data should be saved in the folder `./data`


### Details of Dataset
We followed [COCO](https://cocodataset.org/) format basically.

The structure of the dataset is as follows:
- `train2017`: images for training dataset (like `<id>.jpg`)
- `val2017`: images for validation dataset (like `<id>.jpg`)
- `annotations`: annotations including `instances_train2017.json` and `instances_val2017.json` for training and validation dataset, respectively


## Citation

If you use this code for your research, please consider citing:

```
@article{zheng2021growing,
  title={Growing status observation for oil palm trees using Unmanned Aerial Vehicle (UAV) images},
  author={Zheng, Juepeng and Fu, Haohuan and Li, Weijia and Wu, Wenzhao and Yu, Le and Yuan, Shuai and Tao, Wai Yuk William and Pang, Tan Kian and Kanniah, Kasturi Devi},
  journal={ISPRS Journal of Photogrammetry and Remote Sensing},
  volume={173},
  pages={95--121},
  year={2021},
  publisher={Elsevier}
}
```

Zheng, J., Fu, H., Li, W., Wu, W., Yu, L., Yuan, S., ... & Kanniah, K. D. (2021). Growing status observation for oil palm trees using Unmanned Aerial Vehicle (UAV) images. ISPRS Journal of Photogrammetry and Remote Sensing, 173, 95-121.

## Contact

zjp19@mails.tsinghua.edu.cn

