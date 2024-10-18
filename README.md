# mk_CelebA-HQ_dataset
![Sample Image](imgs/200122.png)
**Change**:
  - python3.6。
  - 自定义保存路径，保存格式PNG。
用于生成 [CelebA-HQ](https://github.com/tkarras/progressive_growing_of_gans) 数据集。
## Usage
### 1. 可以直接修改参数行默认值
  例如：
  p.add_argument(     '-delta_dir',        help='Directory to read CelebA-HQ deltas from', default='a/b/c')
