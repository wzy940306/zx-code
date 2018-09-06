# zx-code

使用步骤：

1.将所需分类的图片（一张或多张）放入face_classifier.exe同文件夹下的test_image文件夹中。

2.点击face_classifier1.0.exe即可对test_image文件夹中的图片进行分类。

3.分类结束后，可打开随后在face_classifier.exe同文件夹下生成的result.txt或打开face_classifier.exe

同文件夹下的result_image文件夹查看分类结果，result_image文件夹内共有16个子文件夹，对应人脸的不同

类。

4.如果说需要二次测试，由于result_image文件夹中的16个子文件夹已经包含了您第一次测试分类后图片，

为避免对您的检验造成干扰，您可以将这16个文件夹先剪切出来保存，然后从空分类中拷贝16个与您刚剪切的

16个文件夹同名的空文件夹放到result_image文件夹中，用来存储第二次测试图片的分类结果，当然您也可以

不这么做。

5.注意，在第二次测试之前将result.txt文件拷贝一份，或者将它重命名，因为程序每次输出结果采取的是如
果result.txt存在，先将其内容清空，再往里写入数据的方法。如果您没有拷贝或者重命名，将会失去第一次
测试的结果。对此造成的不便我们感到十分抱歉。


包含文件简要说明：

1.后缀为.dll的文件是opencv2.4.10为exe文件运行提供的动态链接库。

2.face_classifier.exe是可执行程序，点击即可运行。

3.readme.txt即说明文档。

4.project data文件夹是训练分类器的时候用的，由于分类器已经训练好了，因此使用时无需涉及对此文件夹

的操作。

5.result_image文件夹中的16个子文件夹名分别为：

nothingBoy（什么都不戴，男）, nothingGirl（什么都不戴，女）,onlyhatBoy（只戴帽子，男），

onlyhatGirl（只戴帽子，女），onlyglassesBoy（只戴眼镜，男）, onlyglassesGirl（只戴眼镜，女）, 
onlymasksBoy（只戴口罩，男）,onlymasksGirl（只戴口罩，女）,hatglassesBoy（帽子眼镜，男）,

hatglassesGirl（帽子眼镜，女）, hatmasksBoy（帽子口罩，男） ,hatmasksGirl（帽子口罩，女）,

masksglassesBoy（口罩眼镜，男）,masksglassesGirl（口罩眼镜，女）,allhaveBoy（全戴，男）, 

allhaveGril（全戴，女）

6.test_by_horrible文件夹中放的是我们的实验结果。

7.test_image是您用来放测试图片的文件夹。

8.main.cpp是唯一的源文件，没有写.h文件。