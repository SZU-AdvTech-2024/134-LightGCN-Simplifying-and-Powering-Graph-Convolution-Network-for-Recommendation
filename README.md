### 1. 环境设置

首先，在系统中安装cuda驱动后，创建并激活一个新的 Anaconda 虚拟环境，并安装所需的库：

```
conda create -n light python=3.10
conda activate light
conda install torch
conda install pandas
……
```

### 2. 克隆仓库

从 GitHub 克隆 LightGCN-PyTorch 仓库并进入目录：

```
https://github.com/gusye1234/LightGCN-PyTorch.git 在后面指定路径，或者直接在pycharm命令行进入需要下载仓库的位置进行下载
cd LightGCN-PyTorch-master
#安装依赖
pip install -r requirements.txt
```


### 3. 配置文件

源码文件包中有数据集


### 4. 运行模型

使用以下命令运行训练脚本：

` cd code && python main.py --decay=1e-4 --lr=0.001 --layer=3 --seed=2020 --dataset="gowalla" --topks="[20]" --recdim=64`

dataset部分可以换成别的数据集
