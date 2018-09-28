#Sketch2Code 研究进展
------
通过这几天对Sketch2Code的研究，充分感受到现在科技的发达。

###认识Sketch2Code 
Sketch2Code 是一个能够AI转用户的手稿的接口，这个接口能够将一张图片直接转成一个HTML代码

###转换的过程
- 用户通过网站前端来上传图像
- 自定义视觉模型可预测图像中存在的HTML 元素以及位置。
- 手写文本识别服务读取预测元素内的文本
- 布局算法使用来自预测元素的所有边界框的空间信息来生成适应所有边界框的网格结构。
- HTML生成引擎使用所有这些信息来生成反映结果的HTML标记代码。

在这里我进行了实际的操作和分析。

![](/Users/liangzhe/Desktop/login.jpeg)

Sketch2Code 将手绘草图转换成代码的操作过程。在微软官方网站上可以做更多尝试：[here](https://sketch2code.azurewebsites.net/)

我上传后产生这样的效果
![](/Users/liangzhe/Desktop/login1.png)

左边是我的图，右边是将会生产的页面（这里可以看到，我生成的并不好）
看出来汉字可能不识别，因此我换个图
![](/Users/liangzhe/Desktop/login2.jpeg)
产生了如下的效果，可以看到 已经变的好多了
![](/Users/liangzhe/Desktop/login_result.png)

----
###HTML源代码



<!DOCTYPE html>

<html lang="en">
<head>
    <meta name="viewport" content="width=device-width" />
    <title>HTML Result</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.1/css/bootstrap.min.css" 
          integrity="sha384-WskhaSGFgHYWDcbwN70/dfYBj47jz9qbsMId/iRN3ewGhXQFZCSftd1LZCfmhktB" crossorigin="anonymous">
</head>
<body>
    <div class="container body-content">
        



<div class="container">


                    <div class="row justify-content-start" style="padding-top:10px;">
<label>in</label>



                </div>
                <div class="row justify-content-end" style="padding-top:10px;">
<input class="form-control"></input>


                </div>
                <div class="row justify-content-start" style="padding-top:10px;">

                <div class="col" style="padding-top:10px;">
<label>Use</label>



                </div>
                <div class="col" style="padding-top:10px;">
<input class="form-control"></input>


                </div>
                </div>
                <div class="row justify-content-start" style="padding-top:10px;">

                <div class="col" style="padding-top:10px;">
<label>password : 1</label>



                </div>
                <div class="col" style="padding-top:10px;">
<input class="form-control"></input>


                </div>
                </div>
                <div class="row justify-content-end" style="padding-top:10px;">
<a href="">Login]</a>


                </div>
                <div class="row justify-content-center" style="padding-top:10px;">
<p class="text-black-50">
    Lorem ipsum dolor sit amet, consectetur adipiscing elit
    <br />
    sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
    <br />
    Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris
</p>
                </div>


</div>



    </div>
</body>
</html>

已经自动生成
