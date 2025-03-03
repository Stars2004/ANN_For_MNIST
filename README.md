# 基于 MNIST 的 ANN 图像识别


```
ANN_MINIST_2
├─ 📁data
│  └─ 📁MNIST
│     └─ 📁raw
│        ├─ 📄t10k-images-idx3-ubyte
│        ├─ 📄t10k-images-idx3-ubyte.gz
│        ├─ 📄t10k-labels-idx1-ubyte
│        ├─ 📄t10k-labels-idx1-ubyte.gz
│        ├─ 📄train-images-idx3-ubyte
│        ├─ 📄train-images-idx3-ubyte.gz
│        ├─ 📄train-labels-idx1-ubyte
│        └─ 📄train-labels-idx1-ubyte.gz
├─ 📁images
│  ├─ 📄0.png
│  ├─ 📄1.png
│  ├─ 📄2.png
│  ├─ 📄3.png
│  ├─ 📄4.png
│  ├─ 📄5.png
│  ├─ 📄6.png
│  ├─ 📄7.png
│  ├─ 📄8.png
│  └─ 📄9.png
├─ 📄accuracy.png
├─ 📄ANN.ipynb
├─ 📄ANN模型图参考.jpg
├─ 📄best_model.pth
├─ 📄class_indices.json
├─ 📄demo.ipynb
├─ 📄last_model.pth
├─ 📄loss.png
├─ 📄README.md
└─ 📄result.png
```



结构说明：

1. 📁data 为数据，其中 📁MNIST 为本次实验所使用的手写体数据集，可通过 torchvision 下载；
2. 📁images 为自定义数据集，包含 0 ~ 9 的数字，用于模型预测；
3. 📄ANN.ipynb 为主文件，📄demo.ipynb 是学习资料中提供的示例代码；
4. 📄ANN模型图参考.jpg 为学习资料中提供的 ANN 模型结构示例；
5. 📄accuracy.png 和 📄loss.png 为模型训练、测试的准确率与损失，📄result.png 为模型在自定义数据集上的预测结果；
6. 📄best_model.pth 和 📄last_model.pth 分别为最佳模型参数、最终模型参数；
7. 📄class_indices.json 是包含数据集类别的 json 文件；
8. 📄output.txt 为模型训练时控制台的打印输出，包含训练损失、训练准确率、测试损失、测试准确率；



注：

本实验为方案 4，与方案 3 基本一致，就是将 epoch 从 50 改为 60。
