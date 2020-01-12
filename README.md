# 说明文档
## 编译环境及安装
* 本次大作业采用`Python3.6`编译完成
* 考虑到安装环境比较复杂，故附上`requirement.txt`文件可一键安装运行环境，步骤如下：
> 在项目路径下运行cmd,输入`pip install -r requirements.txt`，等待安装完成即可
## 代码组成及运行方法
### 代码组成
* `calibration.py`为相机内参标定文档，代码从网上参考得来
* `restoration.py`为图像去畸变
* `Featurematching.py`中包括了两幅图像的特征点匹配与初步筛选
* `RANSC.py`（少打了一个A）中为ransac求取基础矩阵
* `plot.py`中为R,t求解与三角化和最后的三维点云重构
* `estimator.py`为第三幅图像的位姿估算与3D-2D关系矩阵求解
* `main.py`为主文档，运行该文档即可

### 运行方法
* 在项目路径下打开cmd，输入`python main.py`即可
* 项目分为两个阶段，第一个阶段为输出点云建模，观察完点云后即可关闭窗口，程序继续运行输出各参数结果

## 其他文件
* `biaoding`中存放相机标定所用的照片
* `matchdemo`中存放匹配所用的三张照片
