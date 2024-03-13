# TEST



## 环境安装 （假设已配置过GeneFace++, 见GeneFace++的TEST.md）

```bash
# MMCV安装
sudo pip3.9 install openmim==0.3.9
sudo mim install mmcv==2.1.0 # 使用mim来加速mmcv安装

sudo pip3.9 install torchshow
sudo pip3.9 install pretrainedmodels
```



## 测试

```bash
python3.9 inference/real3d_infer.py \
--src_img data/raw/examples/Macron.png \
--drv_aud data/raw/examples/Obama_5s.wav \
--drv_pose data/raw/examples/May_5s.mp4 \
--bg_img data/raw/examples/bg.png \
--out_name infer_out/output.mp4 \
--out_mode final

python3.9 inference/app_real3dportrait.py
```