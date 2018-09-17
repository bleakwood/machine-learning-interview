1.给定一首曲子（可能需要手动用audacity等软件更改为wav格式），用madmom找到它所有的重拍（downbeats）

2.假定重拍不在madmom找到的位置（比如说，madmom找到的是所有小节的第一拍，而实际的拍子在所有小节的第二拍），输入实际的重拍，将madmom的所有重拍输出改至指定的位置。举例：
```bash
python3 shift_downbeats.py song.wav 2
```
会将以上的例子找到的小节第一拍全部改为第二拍的时间。

[madmom教程地址](https://github.com/CPJKU/madmom_tutorials)

[madmom在github上的地址](https://github.com/CPJKU/madmom)

[madmom文档](https://madmom.readthedocs.io/en/latest/tutorial.html)

[如何运行教程里的iPython脚本](https://jupyter.readthedocs.io/en/latest/install.html#new-to-python-and-jupyter)

[Python3安装指南（我们目前在用3.6.5）](https://realpython.com/installing-python/)

用于寻找重拍的RNNDownBeatProcessor和DBNDownBeatTrackingProcessor： https://github.com/CPJKU/madmom/blob/master/madmom/features/downbeats.py

可能相关的librosa库（非必须）：https://github.com/librosa/librosa