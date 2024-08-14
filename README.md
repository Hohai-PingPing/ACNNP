# ACNNP
## Novel asymmetric CNN-based and adaptive mean predictors for reversible data hiding in encrypted images

## 摘要

Reversible data hiding in encrypted images (RDHEI) embeds data in the encrypted domain and ensures

that the embedded data can be extracted without errors and the original image can be recovered

losslessly. In many RDHEI methods, local linear predictors are used for image prediction and their

prediction performance remains unsatisfactory in the demand of high embedding capacity. In this

paper, we propose a novel asymmetric CNN-based predictor(ACNNP) which can make full use of

the correlation between neighbouring pixels and greatly improve the prediction accuracy. Then, an

adaptive mean predictor is proposed to cooperate with ACNNP. According to these two predictors,

a two-stage prediction and embedding model is designed to further enhance the embedding capacity

and make the data embedding more flexible. Experimental results demonstrate that the proposed

method achieves average 3.30, 3.46, 2.69 bpp on three common datasets, exhibiting a high embedding

capacity and reversibility while comparing with the state-of-the-art methods. Therefore, this method

provides an effective solution for applications such as privacy protection, copyright preservation, and

data integrity verification.

## 部分代码

### 1. 文件列表

![image-20240814205357733](/Users/baimo/Desktop/HJY_ACNNP 2/assets/image-20240814205357733.png)

### 2. 文件使用说明

* ACNNP_test.py 

  使用训练好的模型，进行像素值预测

* Capacity.py

  计算嵌入容量

* Dataset_new.py  /  Dataset_new_two.py

  加载数据集，两种不同的处理格式，分别用于测试和训练

* NEW_CNN.py

  论文中提出的基于非对称卷积神经网络预测器的网络结构实现

* test

  测试图像

* Train_state240.pth

  训练好的参数

* Train.py

  训练文件

### 3. capacity.py 文件运行示例

**装好环境后，直接运行即可，运行结果如下图所示** （训练不同的轮次，结果会后细微差别）

![image-20240814211024057](/Users/baimo/Desktop/HJY_ACNNP 2/assets/image-20240814211024057.png)

![image-20240814211314113](/Users/baimo/Desktop/HJY_ACNNP 2/assets/image-20240814211314113.png)

### 4. 文章引用方式

| Ping P, Huo J,  Guo B. Novel asymmetric CNN-based and adaptive mean predictors for  reversible data hiding in encrypted images[J]. Expert Systems with  Applications, 2024, 246: 123270. |
| ------------------------------------------------------------ |
|                                                              |

| Ping, Ping, Junyuan Huo, and Bobiao Guo. "Novel asymmetric CNN-based and  adaptive mean predictors for reversible data hiding in encrypted  images." *Expert Systems with Applications* 246 (2024): 123270. |
| ------------------------------------------------------------ |
|                                                              |

| Ping, P., Huo, J., & Guo, B. (2024). Novel asymmetric CNN-based and  adaptive mean predictors for reversible data hiding in encrypted images. *Expert Systems with Applications*, *246*, 123270. |
| ------------------------------------------------------------ |
|                                                              |
