# UODAC
水下物体检测算法赛（光学图像赛道）方案： https://www.kesci.com/home/competition/5e535a612537a0002ca864ac/content/2

## 1. 赛题目的
随着海洋观测的快速发展，水下物体检测别在海军沿海防御任务以及渔业、水产养殖等海洋经济中发挥着越来越重要的作用。水下图像是海洋信息的重要载体，目标检测作为当前人工智能领域的学术热点， 应用前景非常广泛。该技术对于军事活动、资源勘测、海洋噪声污染保护等方面有着巨大的作用。本届算法赛设置的水下光学图像目标检测赛项代表了人工智能和水下机器人技术在未来深度融合的方向。

主要目标： 水下机器人自动检测五种海鲜（海参、海胆、扇贝、海星），或保护或捕捞咱也不知道。

数据样例：
![](https://github.com/ChronousZhang/UODAC/blob/master/1.png)
![](https://github.com/ChronousZhang/UODAC/blob/master/2.png)
![](https://github.com/ChronousZhang/UODAC/blob/master/3.png)

## 2. 数据集
* 训练：5543张jpg图像
* 测试A: 800张jpg图像
* 测试B: 1200张jpg图像


## 3. 方案
* 模型： cascadeRCNN-r50 + cascadeRCNN-SE + cascadeRCNN-x101 
* 融合： WBF
* 数据增强： 裁剪翻转镜像，颜色抖动校准，mixup等

