
# Dive into deep learning

学习[《动手学深度学习》](https://zh-v2.d2l.ai/index.html)

## 环境配置

```shell
conda create --name d2l python=3.9 -y
conda activate d2l

pip install d2l==0.17.6
```

然后到[PyTorch官网](https://pytorch.org/)获取最新版PyTorch GPU版本安装命令：

```shell
pip3 install torch torchvision torchaudio
```


d2l库严格要求一些库的版本号，这里对其进行修改：

```shell
vim {{your_path}}/miniconda3/envs/d2l/lib/python3.9/site-packages/d2l-0.17.6.dist-info
vim METADATA
```

将其中的`==`该为`>=`，如下所示：

```
Requires-Dist: jupyter (>=1.0.0)
Requires-Dist: numpy (>=1.21.5)
Requires-Dist: matplotlib (>=3.5.1)
Requires-Dist: requests (>=2.25.1)
Requires-Dist: pandas (>=1.2.4)
```
