# 首页页面说明

## 第1次

### 目标

* 完成首页顶部导航菜单

### 知识点

* 列表标记以及列表导航

* 垂直居中（line-height）、水平居中

* 伪类选择符

### 代码

HTML

``` html
<html>
    <head>
        <title>轻松批</title>
        <meta charset="utf-8">
        <link rel="stylesheet" href="css/style.css">
    </head>
    <body>
        <div id="wrap">
            <div id="top">
                <div id="content">
                    <div id="top_left">
                        <a href="">
                            <img src="img/logo.png" alt="">
                            <span>让批发更轻松</span>
                        </a>
                    </div>
                    <div id="top_mid">
                        <ul>
                            <li><a href="">首页</a></li>
                            <li>
                                <a href="">服务</a>
                            </li>
                            <li>
                                <a href="">定价</a>
                            </li>
                            <li>
                                <a href="">关于</a>
                            </li>
                        </ul>
                    </div>
                    <div id="top_right">
                        <a href=""><img src="img/h24.png" alt=""></a>
                        <span>123456789</span>
                        <button >立即申请</button>
                    </div>
                </div>
            </div>            
        </div>
    </body>
</html>
```

CSS

``` css
/* *是一个匹配符，匹配所有的选择符 */
*{
    margin: 0px;
}
a{
    text-decoration-line: none;
}
/* ID选择符以#开始 */
#wrap{    
    width: 100%;
    margin: 0 auto;
}
#top{
    width: 100%;
    height: 80px;
    background-color: #000000;
}
#content{
    width: 90%;
    margin: 0 auto;/*居中显示*/
    overflow: hidden;
}
#top_left,#top_mid,#top_right{
    width: 30%;
    float: left;
    overflow: hidden;
}
#top_left img{
    height: 50px;
    float: left;
    padding-top: 15px;   
}
#top_left span{
    height: 80px;
    display: inline-block;
    float: left;
    line-height: 80px;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 20px;
    color: #bcbcca;
}
#top_mid ul{
    list-style: none;
}
#top_mid ul li{
    float: left;
    width: 25%;
    height: 80px;
    line-height: 80px;/*行高*/
    text-align: center;/*水平居中*/
}
#top_mid a{
    font-size: 16px;
    color: white;
}
/* 伪类选择符 */
#top_mid a:hover{
    color: red;
}
#top_right{
    color:white;
    float: right;
}
#top_right img{
    height: 40px;
    padding-top: 20px;
    float: left;
}
#top_right span{
    height: 80px;
    display: inline-block;
    float: left;
    line-height: 80px;
    margin-left: 20px;
}
#top_right button{
    width: 100px;
    height: 40px;
    margin-top: 20px;
    margin-left: 20px;
    background-color: black;
    color: white;
    border-radius: 10px;    
    cursor: pointer;/*改变鼠标形状，手*/
}
#top_right button:hover{
    background-color: #f74906;
    border-color: #f74906;
}
```

## 第2次

### 目标

* 完成首页header和banner部分

### 知识点

* 两列布局（HTML标记：h1、p、input，CSS重点：伪类选择符、border-radius）
* 四列布局（通过ul-&gt;li来实现）

### 代码

HTML

``` html
<html>
    <head>
        <title>轻松批</title>
        <meta charset="utf-8">
        <link rel="stylesheet" href="css/style.css">
    </head>
    <body>
        <div id="wrap">
            ......
            <div id="header">
                <div id="content">
                    <div id="header_left">
                        <h1>批发，从未如此轻松</h1>
                        <p>重新定义批发，为您连接所有客户
                            <br>拥抱移动互联，助您生意再次腾飞</p>
                        <input type="button" value="申请免费试用">
                    </div>
                    <img src="img/p1.png" alt="" class="float_right">
                </div>
            </div>
            <div id="banner">
                <div id="content">
                    <ul>
                        <li>
                            <div id="banner_box">
                                <img src="img/p2.png" alt="">
                                <h3>掌控店铺</h3>
                                <p>实时数据同步，了解店铺运营情况<br>
                                    所有店铺状态，随时随地一手掌握</p>
                            </div>
                        </li>
                        <li>
                            <div id="banner_box">
                                <img src="img/p3.png" alt="">
                                <h3>掌控店铺</h3>
                                <p>实时数据同步，了解店铺运营情况
                                    <br> 所有店铺状态，随时随地一手掌握
                                </p>
                            </div>
                        </li>
                        <li>
                            <div id="banner_box">
                                <img src="img/p4.png" alt="">
                                <h3>掌控店铺</h3>
                                <p>实时数据同步，了解店铺运营情况
                                    <br> 所有店铺状态，随时随地一手掌握
                                </p>
                            </div>
                        </li>
                        <li>
                            <div id="banner_box">
                                <img src="img/p5.png" alt="">
                                <h3>掌控店铺</h3>
                                <p>实时数据同步，了解店铺运营情况
                                    <br> 所有店铺状态，随时随地一手掌握
                                </p>
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </body>
</html>
```

CSS

``` css
......
#header{
    width: 100%;
    background-color: #5f5b5b;
}
#header_left{
    float: left;
    color: #ffffff;
    margin-top: 100px;
}
#header_left h1{
    font-size: 40px;
    font-family: Arial, Helvetica, sans-serif;
    font-weight: 100;
    margin-bottom: 20px;
}
#header_left p{
    line-height: 30px;
    margin-bottom: 20px;
}
#header_left input{
    width: 200px;
    height: 50px;
    cursor: pointer;
    background-color: #f73f3f;
    border:solid 1px #f73f3f;
    border-radius: 25px;
    color: white;
    font-size: 20px;
}
#header_left input:hover{
    background-color: transparent;
    color: #f73f3f;

}
/* 类选择符以.开始 */
.float_right{
    float: right;
}
#header img{
    height: 400px;
}
#banner{
    width: 100%;
    background-color: #0e0e0e;
    padding: 50px 0;
}
#banner ul{
    list-style: none;
    margin: 0 -50px;
}
#banner ul li{
    float: left;
    width: 25%;
}
#banner_box{
    text-align: center;
    color: white;
}
#banner_box h3{
    color: #ef4c4c;
    margin-top: 20px;
    margin-bottom: 5px;
}
#banner_box p{
    font-size: 14px;
}
```

## 第3次

目标

* 完成首页优势和商店两个部分

知识点

* 三列布局（不用ul-li形式，用div设置float形式）
* 选项卡（此部分内容选项卡的功能需要后序学了javascript才能完成时限，目前只实现布局）

代码

HTML新增部分

``` html
<html>
    <head>
        <title>轻松批</title>
        <meta charset="utf-8">
        <link rel="stylesheet" href="css/style.css">
    </head>
    <body>
        <!-- 包裹层 -->
        <div id="wrap">
            .......
            <!-- 优势部分 -->
            <div id="youshi">
                <div id="content">
                    <div id="youshi_header">
                        <h1>三大优势<span class="color_red">祝你生意腾飞</span></h1>
                        <p>我们所做的一切，只为你的生意更好！</p>
                    </div>
                    <div id="youshi_body">
                        <div id="youshi_box">
                            <img src="img/p6.png" alt="">
                            <h3 class="color_red">你的独立网商</h3>
                            <p>即刻拥有你的专属网商平台，扫码访问让你的店铺捧在他的手心里</p>
                        </div>
                        <div id="youshi_box">
                            <img src="img/p7.png" alt="">
                            <h3 class="color_red">你的独立网商</h3>
                            <p>即刻拥有你的专属网商平台，扫码访问让你的店铺捧在他的手心里</p>
                        </div>
                        <div id="youshi_box">
                            <img src="img/p8.png" alt="">
                            <h3 class="color_red">你的独立网商</h3>
                            <p>即刻拥有你的专属网商平台，扫码访问让你的店铺捧在他的手心里</p>
                        </div>
                    </div>
                </div>
            </div>
            <!-- shop部分 -->
            <div id="shop">
                <div id="content">
                    <div id="shop_header">
                        <span class="active">云商店</span>
                        <span>进销存</span>
                        <span>商米v1</span>
                    </div>
                    <div id="shop_body">
                        <div id="shop_body_left">
                            <h1>你独有的网店<span class="color_red">-轻松批云商店</span></h1>
                            <p>轻松批展示店专为批发商进行开发，让您拥有独立的、安全的展示空间，
                            所有数据直接在APP上即可进行编辑，提供全面的展示、交易、售后服务，为您的批发事业插上互联网的翅膀！</p>
                            <p class="font_weight">无限容量空间<br>一键生成二维码<br> 免费公众号服务</p>
                            <button>进入示范店铺</button>                            
                        </div>
                        <img src="img/p9.png" alt="">
                    </div>
                </div>
            </div>

        </div>
    </body>
</html>
```

CSS新增部分

``` css
.......
/*优势部分*/
#youshi{
    background-color: #e2e2e8;
}
#youshi_header{
    text-align: center;
    margin: 70px 0;
}
.color_red{
    color: #e46e6e;
}
#youshi_body{
    margin-bottom: 100px;
    width: 100%;
    overflow: hidden;/*清除youshi_body里面元素浮动对后序元素的影响*/
}
#youshi_box{
    float: left;
    width: 23%;
    text-align: center;
    border: solid 1px #f15252;
    padding: 30px;
    margin: 0 20px;
    border-radius: 10px;
}
#youshi_box img{
    height: 100px;
}

/*商务部分*/
#shop_header{
    text-align: center;
    margin: 50px 0;
}
#shop_header span{
    display: inline-block;
    width: 100px;
    height: 40px;
    line-height: 40px;
    background-color: #d06d6d;
    margin: 0 20px;
    border-radius: 20px;
    color: white;
}
#shop_header span.active{
    background-color: #978686;
}
#shop_body{
    margin-bottom: 30px;
    width: 100%;
    overflow: hidden;
}
#shop_body_left{
    float: left;
    width: 50%;
}
#shop_body img{
    float: right;    
}
#shop_body_left h1{
    margin-bottom: 50px;
    font-size: 30px;
    font-family: Arial, Helvetica, sans-serif;
    font-weight: 100;
}
#shop_body_left p{
    margin-bottom: 30px;
    color: #827b7b;
}
#shop_body_left p.font_weight{
    font-weight: 900;
}
#shop_body_left button{
    width: 200px;
    height: 50px;
    border-radius: 10px;
    background-color: #d06d6d;
    border: solid 1px #d06d6d;
    cursor: pointer;
    color: white;
    font-size: 20px;
}
#shop_body_left button:hover{
    background-color: transparent;
    color: #d06d6d;
}
```

## 第4次

### 目标

* 完成首页帮助部分以及表单知识点的学习

### 知识点

* css属性：text-indent，分割线
* 表单（HTML5属性和表单标记）

### 代码

表单HTML代码

``` html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">   
    <title>Document</title>
</head>
<body>
    <form action="">
        <label for="yh">文本框：</label><input type="text" name="" id="yh" placeholder="昵称"><br>
        <label for="mm">密码框：</label><input type="password" name="" id="mm"><br>
        性别：<input type="radio" name="sex" id="">男<input type="radio" name="sex" id="">女<br>
        爱好：<input type="checkbox" name="aihao" id="">足球
                <input type="checkbox" name="aihao" id="">蓝球
                <input type="checkbox" name="aihao" id="">排球<br>
        生日：
        <select name="birth" id="">
            <option value="1">1991年</option>
            <option value="2">1992年</option>
            <option value="3">1993年</option>
            <option value="4">1994年</option>
        </select><br>
        <input type="date" name="" id=""><br>
        <input type="email" name="" id="" placeholder="邮箱"><br>
        <input type="file" name="" id=""><br>        
        <input type="tel" name="" id=""><br>
        <input type="submit" value="提交">
        <input type="reset" value="重置">
        <input type="button" value="取消" onclick="">
    </form>
</body>
</html>
```

首页帮助部分HTML代码

``` html
<!-- 帮助部分 -->
            <div id="help">
                <div id="content">
                    <h1>我们如何帮助客户成功</h1>
                    <div id="help_body">
                        <img src="img/p14.png" alt="">
                        <div id="help_body_right">
                            <p>轻松批让我不再像以前一样每天都要守在店里观察客户情况，在家里打开手机就可以看到店铺整体的业务情况，让我有更多时间在面料、工厂和款式上下功夫，自带的销量库存报告让我可以很准确的进货下单</p>
                            <p>并且轻松批提供的网上店铺，更方便我的客户看新款，我也不用发微信来骚扰客户，现在的老客户越来越多！用轻松批，说老实话并没有轻松多少，但是生意变好了很多！继续加油！！！</p>
                            <div id="help_right_box">
                                <div id="help_right_box_left">
                                    <h3>特朗普</h3>
                                    <p class="help_p_teshu">味道档口老板，美衣城C071档</p>
                                </div>
                                <span>WeiDao</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
```

首页帮助部分CSS代码

``` css
/* 帮助部分 */
#help{
    width: 100%;
    background-color: #dad6d6;
}
#help h1{
    text-align: center;
    color: #bf2f2f;
    font-weight: 100;
    padding-top: 100px;
    padding-bottom: 50px;
    border-bottom: solid 1px #8c8787;
}
#help_body{
    width: 100%;
    overflow: hidden;/*由于里面的内容设置了浮动，所以要清楚浮动对后序元素的影响*/
    margin-top: 50px;  
    margin-bottom: 50px;  
}
#help_body img{
    width: 200px;
    border-radius: 100px;
    float: left;
    margin-left: 50px;
}
#help_body_right{
    width: 700px;
    float: right;
    margin-right: 50px;
}
#help_body_right p{
    font-size: 14px;
    color: #736e6e;
    text-indent: 2em;
}
#help_right_box{
    width: 100%;
    overflow: hidden;
    margin-top: 50px;
}
#help_right_box_left{
    float: left;
}
#help_right_box span{
    float: right;
    text-transform: uppercase;
    font-style: italic;
    margin-right: 50px;
    font-size: 30px;
}
#help_right_box_left h3{
    color: #d65e5e;
}
#help_body_right p.help_p_teshu{
    color: #d65e5e;
    text-indent: 0em;
}
```

## 第5次

### 目标

完成轻松批首页表单部分、footer部分和尾部部分

### 知识点

* 表单，textarea标记
* 尾部四列布局（ul-li）

### 代码

首页表单部分HTML代码

``` html
<!-- 表单部分 -->
            <div id="form">
                <div id="content">
                    <div id="form_left">
                        <h1>留下您的电话，我们第一时间联系您</h1>
                        <form action="">
                            <input type="text" name="" id="" placeholder="姓名">
                            <input type="tel" name="" id="" placeholder="电话号码"><br>
                            <input type="email" name="" id="youxiang" placeholder="邮箱"><br>
                            <textarea name="" id="" rows="10" placeholder="内容"></textarea><br>
                            <input type="submit" value="提交" class="submit">
                        </form>
                        <span>温馨提示：可以在内容中填写您的店铺地址，在开通业务的地区，我们提供上门服务！</span>
                    </div>
                    <img src="img/p12.png" alt="" class="float_right">
                </div>
            </div>
```

首页表单部分CSS代码

``` css
/* 表单部分 */
#form{
    width: 100%;
    background-color: white;
    padding: 50px 0;
}
#form_left{
    float: left;
}
#form_left h1{
    color: red;
    font-weight: 100;
    margin-bottom: 30px;
}
#form_left input{
    width: 250px;
    height: 40px;
    margin-bottom: 20px;
}
#form_left input#youxiang{
    width: 505px;
}
#form_left textarea{
    width: 505px;
    height: 100px;
    margin-bottom: 20px;
}
#form_left input.submit{
    background-color: red;
    border: solid 1px red;
    color: #fff;
    font-size: 26px;
    cursor: pointer;
}
#form_left input.submit:hover{
    background-color: palevioletred;
}
#form_left span{
    color:#dad6d6;
    font-size: 14px;
}
```

首页footer部分和底部部分HMTL代码

``` hmtl
<!-- footer部分 -->
            <div id="footer">
                <div id="content">
                    <span>轻松批，让批发更轻松！！！</span>
                    <input type="button" value="免费试用版本">
                </div>
            </div>
            <!-- 底部部分 -->
            <div id="bottom">
                <div id="content">
                    <ul>
                        <li>
                            <h3>关于我们</h3>
                            <p>轻松批是广州市晶焰网络科技有限公司专为批发行业开发的成套批发管理工具，我们致力于解决批发行业的各种痛点，并为客户提供更好和更优质的产品。</p>
                        </li>
                        <li>
                            <h3>合作伙伴</h3>
                            <p class="color_green">阿里云--阿里巴巴网络服务平台</p>
                            <p>商米--小米控股商用设备提供商</p>
                        </li>
                        <li>
                            <h3>联系方式</h3>
                            <p>
                                <img src="img/1-email.png" alt="">
                                <span>qsp@baokuant.com</span>
                            </p>                            
                            <p>
                                <img src="img/1-phone.png" alt="">
                                <span>+86 13826027418</span>
                            </p>
                            <p>
                                <img src="img/1-address.png" alt="">
                                <span>广州市越秀区人民南路88号肯德基二楼</span>
                            </p>
                        </li>
                        <li>
                            <h3>帮助与支持</h3>
                            <p>
                                <img src="img/1-list.png" alt="">
                                <span>使用帮助</span>
                            </p>
                            <p>
                                <img src="img/1-phone.png" alt="">
                                <span>+86 13826027418</span>
                            </p>
                            <p>
                                <img src="img/1-address.png" alt="">
                                <span>广州市越秀区人民南路88号肯德基二楼</span>
                            </p> 
                        </li>
                    </ul>
                </div>
            </div>
```

首页footer部分和底部部分CSS代码

``` css
/* footer部分 */
#footer{
    background-color: #000000;
    padding: 30px 0;
    color: white;
}
#footer span{
    height: 60px;
    line-height: 60px;
    display: inline-block;
    color: #dad6d6;
    font-style: italic;
}
#footer input{
    float: right;
    background-color:#D7551A;
    width: 200px;
    height: 60px;
    border: solid 1px #D7551A;
    border-radius: 30px;
    cursor: pointer;
    color: white;
}
#footer input:hover{
    background-color: transparent;
}
/* 底部部分 */
#bottom{
    width: 100%;
    background-color: #333435;
    color: white;
    padding: 40px 0;
}
#bottom ul{
    list-style: none;
    width: 100%;
    overflow: hidden;
    padding: 0;
}
#bottom ul li{
    float: left;
    width: 23%;
    margin-right: 20px;
}
#bottom ul li h3{
    color: #c3c0cf;
    font-weight: 100;
    /* font-size: 24px; */
    margin-bottom: 20px;
}
#bottom ul li p{
    color: #c3c0c0;
    font-size: 14px;
}
#bottom ul li span,p{
    /* display: block; */
    color: #c3c0c0;
    font-size: 14px;
}
#bottom ul li p.color_green{
    color: green;
    margin-bottom: 20px;
}

#bottom ul li img{
    height: 25px;
    float: left;
}
#bottom ul li p span{
    display: inline-block;
    height: 25px;
    margin-bottom: 10px;
    margin-left: 10px;
}
```
