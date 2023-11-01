运行方式:
        (1)将图像JPG文件放在VOCData/images文件夹下，同时，将对应的xml文件放在VOCData/Annotations文件夹下
        (2)运行xml_to_yolo.py将xml文件转换为txt文件，之后运行split_train_val.py文件，分割数据集为训练集和 
        测试集以及验证集.
        (3)运行train.py文件，进行训练
        (4)修改detect.py文件参数，将训练出来的模型导入预测，本代码已经导入了runs/train/exp文件夹下的模型， 
        该模型由1000个数据集，120个epoch训练出来，预测效果较好
        (5)将要预测的图片放入data/images中，之后就可以用detect.py文件进行预测
