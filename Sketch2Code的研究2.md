#关于Sketch2Code的调查研究
---
2018年以来，人工智能的研究越来越活热，年初名列GitHub排行榜TOP1的项目是Screenshot-to-code-in-Keras，这个项目中，研究者通过利用神经网络来完成深度学习，自动把设计稿编程HTML和CSS代码。
Emil Wallner也写过一篇论文《Turning Design Mockups Into Code With Deep Learning》，讲述了他自己是如何根据Pix2code等论文构建了一个强大的前端代码的生成模型，并且讲了利用LSTM与CNN，将设计原型编写为HTML和CSS网站的过程。

在这篇论文之后，Airbnb则推出了**sketch2code**

在Sketch2Code的introducation中也给中了实际训练的网站。
客户只要上传5张以上的图片就可以让计算机进行深度学习从而给出了前端代码
![](https://ss.csdn.net/p?http://mmbiz.qpics.cn/mmbiz_png/Pn4Sm0RsAuhNKRusVIjUFp6ibMB2Phbc0kEEOkyz5dkfJCwO3zuYxOXy0cIrAXS4HehD3DndaKognFvMQ90ZFEA/640?wx_fmt=png&wxfrom=5&wx_lazy=1)
然后通过神经网络把设计训练图转化为HTML代码。
![](https://ss.csdn.net/p?https://mmbiz.qpic.cn/mmbiz_gif/Pn4Sm0RsAuhNKRusVIjUFp6ibMB2Phbc0KPWzP8GoB5TiaiaiakxffOjYEl2SJkRsXyH5ia0GQgRjqwfFFnP7LUuG6g/640?wx_fmt=gif)