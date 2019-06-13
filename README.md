## 1、feature_map_fusion
双分支特征图融合的异源图像匹配方法

## train_nature_X.py：训练和测试的代码；model_d_X：模型的代码

**tensor:** 双分支网络结构（参数共享）     
**tensor_no:** 双分支网络结构（参数不共享）     
**2ch:** 双通道网络结构        
**map32:** 双分支特征图融合的网络结构（参数共享）      
**map32_no:** 双分支特征图融合的网络结构（参数不共享）       
**map32_diff:** 双分支特征图差值融合的网络结构

## 简介：
基于特征图差值融合的异源图像块匹配方法。针对异源图像提取的特征信息表达能力不足的问题，通过特征图融合的方式将空间邻域信息引入到图像特征描述子中，充分提取利用图像的有效信息。为解决特征描述子中存在的鉴别性差异信息容易被忽视的问题，本文在特征图融合方法的基础上进行改进，利用特征图组求差值的方式得到残差特征图，之后进行匹配度量。该策略不仅提高了网络对重要匹配特征的关注力度，而且增加了网络自身的稀疏性，提高了匹配准确率和网络健壮性。

First, heterogeneous image patches matching method based on feature map fusion. Aiming at the problem that the expressivity of the feature information extracted from heterogeneous image is insufficient, the spatial neighborhood information is introduced into the image feature descriptor through feature map fusion, and the valid information of the image is fully extracted. In order to solve the problem that the discrepancy information in the image descriptor is easily neglected, this paper improves on the feature map fusion method. In this way, the residual feature map is obtained by using the difference between feature maps, and then image patches are compared accordingly. The strategy not only enhances the network's attention to the key matching features, but also increases the sparseness of the network itself. As a result, the image patches matching accuracy and network robustness have been improved.
