 https://github.com/Hironsan/BossSenso
参考了这个日本工程师的代码

1.获取训练集 打开pick_face.py 
2.dateset dataset下会分几个文件夹，你想让你的模型识别几张人脸就建立几个子文件夹每个子文件夹里面应该有至少几十张照片。然后进入train_model.py
3.模型训练好之后，打开read_camera.py，这个文件中有一个Camera_reader的类，在模型初始化的时候就加载你之前训练好的模型。
4.然后建立一个Camera_reader的实例之后调用build_camera（）的方法，该方法打开摄像头，并对视频流中读取到的人脸交给model进行识别：
