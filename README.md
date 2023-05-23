# chinese_tea_dataset
用于中国茶机器学习的数据集。

**写在前面，数据质量很差**

3.2 数据集的采集与处理
通过整理购物网站的分类数据,得出中国的茶叶大致分为绿茶、乌龙茶、红茶、白茶、黑茶这五个大类；进一步分析销售数据得到集中广受消费者青睐的茶叶种类，如龙井、安溪铁观音、金骏眉、寿眉白茶、碎银子等，将它们作为深度学习的对象。
确定要进行学习的茶叶种类后，从Google图片、Bing图片、普洱茶网搜集并人为筛选了5个大类、20个小类，共计600余张的茶叶样本，样本例如图3.1所示；每个小类有30张样本，按照8：2的比例将其分为测试集与训练集进行训练。采集的茶叶样本存在着样本数量少、分辨率不统一、干扰信息多等问题，所以有必要在每轮训练前对茶叶样本进行缩放、随机裁剪、随机水平翻转操作进行数据增强，如图3.2数据增强与未增强对比所示。