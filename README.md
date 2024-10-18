# mk_CelebA-HQ_dataset
![Sample Image](imgs/200122.png)
**Change**:
  - python3.6。
  - 自定义保存路径，保存格式PNG。

用于生成 [CelebA-HQ](https://github.com/tkarras/progressive_growing_of_gans) 数据集。
代码基于 [celeba-hq-modified](https://github.com/willylulu/celeba-hq-modified/tree/master) ，进行了略微修改。

CelebA-HQ 数据集是在 ICLR2018 由 NVIDIA 在 [《Progressive Growing of GANs for Improved Quality, Stability, and Variation》](https://arxiv.org/abs/1710.10196) 中提出，其中包含30k张1024分辨率图像。
## Usage
**First**
1. 克隆本仓库

        git clone https://github.com/willylulu/celeb-hq-modified

2. 准备好必需文件

  ```bash
  celeba_dir
  ├── img_celeba
      ├── 000001.jpg
      ├── 000002.jpg
      ...
  ├── Anno
      └── list_landmarks_celeba.txt
  
  delta_dir
  ├── image_list.txt
  ├── deltas00000.zip
  ├── deltas01000.zip
      ...
  └── deltas29000.zip
  
  ```


**Second**

  1. 可以直接修改参数行默认值 default=''
  
  **例如**：
  
      p.add_argument(    '-create_what', help='what dataset', default='celebahq')
      
      p.add_argument(     '-h5_filename',      help='HDF5 file to create', default='123456.h5')
      
      p.add_argument(     '-celeba_dir',       help='Directory to read CelebA data from', default='/a/b/e')
      
      p.add_argument(     '-delta_dir',        help='Directory to read CelebA-HQ deltas from', default='/a/b/d')
      

  进一步终端中执行：
  
      python <path_of_h5tool.py>
  
  2. 直接在终端中运行
  
      cd <dir_of_h5tool.py>
      
      python h5tool.py --celeba_dir <path_to_celeba> --delta_dir <path_to_delta>

## Reference
[tkarras/progressive_growing_of_gans](https://github.com/tkarras/progressive_growing_of_gans)

[CelebA](https://mmlab.ie.cuhk.edu.hk/projects/CelebA.html)

[willylulu/celeba-hq-modified](https://github.com/willylulu/celeba-hq-modified/tree/master)
