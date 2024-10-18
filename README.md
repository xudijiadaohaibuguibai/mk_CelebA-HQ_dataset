# mk_CelebA-HQ_dataset
![Sample Image](imgs/200122.png)
**Change**:
  - python3.6。
  - 自定义保存路径，保存格式PNG。

用于生成 [CelebA-HQ](https://github.com/tkarras/progressive_growing_of_gans) 数据集。
代码基于 [celeba-hq-modified](https://github.com/willylulu/celeba-hq-modified/tree/master) ，进行了略微修改。
## Usage
### 1. 可以直接修改参数行默认值
  **例如**：
  p.add_argument(    '-create_what', help='what dataset', default='celebahq')
  
  p.add_argument(     '-h5_filename',      help='HDF5 file to create', default='123456.h5')
  
  p.add_argument(     '-celeba_dir',       help='Directory to read CelebA data from', default='/a/b/e')
  
  p.add_argument(     '-delta_dir',        help='Directory to read CelebA-HQ deltas from', default='/a/b/d')
  
  p.add_argument(     '-delta_dir',        help='Directory to read CelebA-HQ deltas from', default='/a/b/c')
