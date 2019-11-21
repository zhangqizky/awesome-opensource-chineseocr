# Chinese Text Detection(not include recognition) 

## Awesome list
### CTPN: [Detecting Text in Natural Image with Connectionist Text Proposal Network](https://arxiv.org/pdf/1609.03605.pdf)

CTPN是目前流传最广、影响最大的开源文本检测模型，可以检测水平或微斜的文本行。文本行可以被看成一个字符sequence，而不是一般物体检测中单个独立的目标。同一文本行上各个字符图像间可以互为上下文，在训练阶段让检测模型学习图像中蕴含的这种上下文统计规律，可以使得预测阶段有效提升文本块预测准确率。CTPN模型的图像预测流程中，前端使用当时流行的VGG16做基础网络来提取各字符的局部图像特征，中间使用BLSTM层提取字符序列上下文特征
，然后通过FC全连接层，末端经过预测分支输出各个文字块的坐标值和分类结果概率值。在数据后处理阶段，将合并相邻的小文字块为文本行。

- [chinese_ocr](https://github.com/YCG09/chinese_ocr)
keras+tensorflow版本的实现，git clone之后就能跑，效果还不错，2000*2000左右的图像6s左右一张
- 
### PSENet：[Shape Robust Text Detection with Progressive Scale Expansion Network](https://arxiv.org/pdf/1806.02559.pdf)

- [PSENET](https://github.com/xiaomaxiao/PSENET)
