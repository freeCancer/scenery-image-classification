# scenery-image-classification
对像素大小不一的15类、1500张风景图片，学习使用多种模型方法训练分类。
Run1：采取简单的缩小图像来提取特征，使用KNN分类器；
Run2：采取密集采样从图片提取特征，使用minibatch Kmeans聚类所有特征并以此建立词袋模型的特征库，再使用线性svm分类；
Run3：采取sift提取特征，使用fisher vector进行编码，再利用线性svm分类；
Run3-transfer：采取迁移学习，调用训练好的ResNet50深度学习模型，并微调。
