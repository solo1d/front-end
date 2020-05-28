## 目录

- [骨架](#骨架)
- [转义字符](#转义字符)
- [排版标签](#排版标签)
    - [h1标题标签](h1标题标签)
    - [ul有序和ol无序列表标签](#ul有序和ol无序列表标签)
    - [center,em,strong,del,ins等文字样式标签](#center,em,strong,del,ins等文字样式标签)
    - [p段落标签](#p段落标签)
    - [hr水平线标签](#hr水平线标签)
    - [br换行标签](#br换行标签)
- [a超链接标签](#a超链接标签)
- [img图片标签](#img图片标签)
- [table表格标签](#table表格标签)
    - [col设置一列数据显示格式](#col设置一列数据显示格式)
    - [colgroup设置一组数据显示格式](#colgroup设置一组数据显示格式)
    - [tr表格中的行](#tr表格中的行)
    - [td行中的列](#td行中的列)
    - [th行中的列,简化](#th行中的列,简化)
- [input输入框或按钮,提交表单案例,有form标签](#input输入框或按钮,提交表单案例,有form标签)
    - [get请求和post请求,提交数据和获取数据的表单补充内容](#get请求和post请求,提交数据和获取数据的表单补充内容)
- [span容器和div容器标签](#span容器和div容器标签)
- 



## 骨架

```html
<!DOCTYPE html>     <!-- 声明使用的html 版本. 写在 <html> 标签之前 -->
<html lang="zh-Hans">     <!--语言标签解释 为简体中文 -->
	<meta charset="UTF-8" />     <!-- 声明使用的 unicode  UTF-8 字符集,写在紧挨着 html 那里-->      
    <head> </head>    <!-- 头标签 用于存放:  title , mete , base,  style ,script ,link  -->
    <body>    <!-- 主体 -->
       <title> 标签 标题 </title>
       <table>
      		 <col/>
           <colgroup>
          	  <tr>
               	<td> <input /> </td>
                <th></th>
              </tr>
            </colgroup>
          </table>
				<a> <img /> </a>
    </body>
</html>
```

- **`html`** 标签  ,  **根标签**
    - 所有 html 中标签的一个根节点.
- **`head`** 标签 ,  **头标签**
    - 用于存放:  title , mete , base,  style ,script ,link 
- **`title`**  标签 ,  **标题标签, (显示到浏览器标签部分)**
    - 让页面拥有一个属于自己的标题
- **`body`** 标签,  **主体标签**
    - 页面的主体部分, 用于存放所有的 html 标签.



## 转义字符

```html
&nbsp;     <!-- 网页上显示一个空格 是 html的空格转义字符 -->
```



## 排版标签

### h1标题标签

```html
<h1 align="center"> ... </h1>  <!-- 标题标签  最大, 没有特殊符号, 后面属性代表居中显示-->
<h6> ... </h6>  <!-- 标题标签  最小, 没有特殊符号-->

<!-------------------- 显示效果 ------------------------------------------->
<!DOCTYPE html> 
<html lang="zh-Hans">
  <meta charset="UTF-8" />
  <head> <titele> 标签 </titele> </head>
  <doby>
    <h1>最大的标签</h1>
    <h6>最小的标签</h6>
  </doby>
</html>
```

<img src="image/标签h1.png" alt="标签h1.png" style="zoom:50%;" />



### ul有序和ol无序列表标签

```html
<ul> <li> 列表项目 </li> </ul>  <!-- ul 这只个列表,是无序列表,前面只有个实心圆.里面需要列表项进行填充 -->
<ol> <li> 列表项目 </li> </ol>  <!-- ul 这只个列表,是有序列表,前面有数字来显示.里面需要列表项进行填充 -->

<!-------------------- 显示效果 ------------------------------------------->
<!DOCTYPE html>
<html lang="zh-Hans">
  <meta charset="UTF-8" />
  <head> <title> ul , li </title>  </head>
  <body>
    <ul> <li> 列表1</li> </ul>
    <ol> <li> 列表2</li> </ol>
  </body>
</html>
```

<img src="image/列表标签.png" alt="列表标签" style="zoom:50%;" />



### center,em,strong,del,ins等文字样式标签

```html
<center> ... </center>  <!-- 居中效果 -->
<em> ... </em>          <!-- 文字以 斜体 方式显示 -->
<strong> ... </strong>  <!-- 文字以 粗体 的方式显示 -->
<del> ... </del>        <!-- 文字以加 删除线 方式显示 -->
<ins> ... </ins>        <!-- 文字以 加下划线 方式显示 -->

<!-------------------- 显示效果 ------------------------------------------->
<!DOCTYPE html>
<html>
  <meta charset="UTF-8" />
  <head> <title> center,em,strong,del,ins </title>  </head>
  <body> 
    <ul> <li> <center><strong><em>居中加粗和斜体 </em></strong>  </center> </li> </ul>
    <ol> <li> <del> <ins> >删除线和下划线  </ins></del> </li> </ol>
  </body>
</html>
```

<img src="image/文字样式.png" style="zoom:50%;" />



### p段落标签

```html
<p> ... </p>     <!--段落标签, 文字会独占一行 , 跟换行符差不多--> 

<!-- p标签是   paragraph 的缩写-->
```



### hr水平线标签

```html
<hr/>            <!-- 水平线-->
<hr color="yellow" />    <!-- 设置颜色-->

<!-- hr 是 horizontal 横线的缩写,  是单标签-->

<!-------------------- 显示效果 ------------------------------------------->
<!DOCTYPE html>
<html lang="zh-Hans">
	<meta charset="UTF-8" />
	<head> 
		<title>hello</title>
	</head>
	<body>
		<hr color="red" />	<p>这是第一段</p>  <hr color="yellow" /> <hr color="purple" />
		<hr color="green" />
	</body>
</html>
```

<img src="image/水平线标签.png" alt="水平线标签" style="zoom:50%;" />



### br换行标签

```html
<br/>            <!-- 换行标记 , 文字会换行-->
<!-- br 是 break 打断,换行 的缩写,是单标签 -->
```



## a超链接标签

```html
<!-- 超链接  , 可以嵌套图片, 文本,等很多内容 -->
<a href="链接地址" target="_blank" style="text-decoration: none;margin: 0 15px color: black;"> 文本或图片 
</a>   
   <!-- target表示目标地址,可以是目录 也可以是某个网址 -->
   <!-- _blank参数表示空白, 代表在空白新窗口打开链接地址页面,没有该参数就在当前页面跳转 -->
   <!-- 嵌套图片的话, 就要写上 <img /> 标签了
   <!-- style="margin: 0 15px;"   设置文本的上下距离为0, 左右距离为15px -->
   <!-- style="text-decoration: none;"    取消超链接底部的下下划线 -->
   <!-- border-right: solid 1px #808080; 边框样式为直线,但只保留右边框,边框粗细, 边框颜色 -->
   <!-- padding: 0px 15px;  内边距 上下增加0高度, 左和右都增加 15px宽度 -->


<!-------------------- 显示效果 ------------------------------------------->
<!DOCTYPE  html>
<html>
    <meta charset="UTF=8" />
    <head><title>超链接</title> </head>
    <body> <a href="html/index.html" target="_blank" >  <img src="img/1.png" /> 链接 </body>
</html>
```

<img src="image/超链接.png" alt="超链接" style="zoom:50%;" />



## img图片标签

```html
<!-- 显示图片,从左到右, 以底部为基准进行排列 ----------------------->
<img src="图片地址" width="50px" />      <!-- px是单位 代表像素 -->
<img src="图片地址" width="100%" />     <!-- 100% 代表撑满整个窗口,但不会出现移动条 -->
<img src="图片地址" title="鼠标放在图片上之后出现的提示"  alt="图片加载失败后出现的文字" />

<!-------------------- 显示效果 ------------------------------------------->
<!DOCTYPE  html>
<html>
    <meta charset="UTF=8" />
    <head><title>图片</title> </head>
    <body> <img src="img/1.png" width="40px" title="1.png" alt="失败了" /> </body>
</html>
```

<img src="image/图片.png" style="zoom:50%;" />

## table表格标签

```html
<!--    表格       -->
<table border="1px" cellspacing="0" width="600px" height="100px" >  
    <!-- 添加并设置边框为1像素 , 单元格间距设置为0 去掉重复框, 设置所有行列都是600宽度 ,100高度-->
    
<tbody></tbody>
    <!-- 表格中的内容, 应该写在这个标签内 -->
```

### col设置一列数据显示格式

```html
<col width="200xp" />   <!-- 设置每行的第一列的宽度为200像素点 -->

<!-------------------- 显示效果 ------------------------------------------->
<!DOCTYPE  html>
<html>
    <meta charset="UTF=8" />
    <head><title>表格col</title> </head>
    <body>
        <table   border="1px" cellspacing="0" >
            <tbody>
            <col width="100xp"/>  <!-- 设置每行的第一列 -->
            <col width="300xp" />  <!-- 设置每行的第二列 -->
            <tr> <td> 第一行</td><td>一行二列</td> </tr>
            <tr> <td> 第二行</td>  </tr>
            <tr> <td> 第三行</td> <td>三行二列</td> </tr>
            </tbody>
        </table>
    </body>
</html>
```

<img src="image/col表格.png" style="zoom:50%;" />



### colgroup设置一组数据显示格式

```html
<colgroup span="6" width="100xp" ></colgroup>
     <!-- 设置每行的前6列为100像素宽度 -->


<!-------------------- 显示效果 ------------------------------------------->
<!DOCTYPE  html>
<html>
    <meta charset="UTF=8" />
    <head><title>表格col</title> </head>
    <body>
        <table   border="1px" cellspacing="0" >
            <tbody>
            <colgroup width="200xp" span="3" ></colgroup>  <!-- 设置每行的前3列为200像素宽度 -->
            <tr> <td> 第一行</td><td>一行二列</td><td>一行三列</td><td>一行四列</td> </tr>
            <tr> <td> 第二行</td>  </tr>
            <tr> <td> 第三行</td> <td>三行二列</td> </tr>
		    <tr> <td> 第四行</td> <td>四行二列</td> </tr>	
            </tbody>
        </table>
    </body>
</html>
```

<img src="image/colgroup表格.png" style="zoom:50%;" />

### tr表格中的行

```html
<tr height="40px" align="center" >  <td></td> </tr>
      <!-- 填写这一行所有的元素,设置该行内容居中, 占据高度40xp -->

<!-------------------- 显示效果 ------------------------------------------->
<!DOCTYPE  html>
<html>
    <meta charset="UTF=8" />
    <head><title>表格col</title> </head>
    <body>
        <table   border="1px" cellspacing="0" >
            <tbody>
            <tr  > <td > 第一行</td><td>一行二列</td><td>一行三列</td><td>一行四列</td> </tr>
            <tr height="40px" align="center"> <td width="130px"> 第二行</td>  </tr>
            <tr> <td> 第三行</td> <td>三行二列</td> </tr>
		    <tr> <td> 第四行</td> <td>四行二列</td> </tr>	
            </tbody>
        </table>
    </body>
</html>
```

<img src="image/tr表格行标签.png" style="zoom:50%;" />

### td行中的列

```html
<td  width="200px" align="center" colspan="7" rowspan="3" >  </td>  
		<!-- 填写这一列的元素,设置空间和居中, 让这个单元 合并一行中的7列, 再合并一列中的 3行-->
        <!-- align属性有 : center居中, right右对齐, left左对齐
<!-------------------- 显示效果 ------------------------------------------->
<!DOCTYPE  html>
<html>
    <meta charset="UTF=8" />
    <head><title>表格col</title> </head>
    <body>
        <table   border="1px" cellspacing="0" >
            <tbody>
            <tr> <td> 第一行</td><td>一行二列</td><td>一行三列</td><td>一行四列</td> </tr>
            <tr> <td colspan="4" align="center"> 第二行</td>  </tr>
            <tr> <td> 第三行</td> <td>三行二列</td> <td rowspan="3" colspan="2">这里</td></tr>
		    <tr> <td> 第四行</td> <td>四行二列</td> </tr>	
            </tbody>
        </table>
    </body>
</html>
```

<img src="image/td表格列标签.png" style="zoom:50%;" />

### th行中的列,简化

```html
<th> c </th>  <!-- th等同于 加粗并水平居中的 td -->
```



## input输入框或按钮,提交表单案例,有form标签

```html
<input type="text" , value="提交" name="user" />
    <!-- value 显示的内容, name 变量名,通过设置可以变成输入框和按钮 -->
    <!-- type 显示属性包括:  text文字文本, password密码框, button无效按钮, radio单选框, checkbox复选框,
                       submit提交按钮,  reset重置按钮, file文件选择框 ,select下拉框 , time时间-->
    <!-- input标签必须放在 form标签内一起使用,进行表单的提交 -->

<form action="网址" method="get" ></form>
   <!-- 必须要有 action标签, 属性是把表单提交给哪个地址 -->
   <!-- method属性为 get 是获取数据到本地的请求,  post是提交数据到服务器
   <!-- 所有需要提交的数据, input 必须有name属性



<!-------------------- 显示效果 ------------------------------------------->
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
<!-- form action提交表单的地址, 必须要填写 -->
<!-- 点击提交后,网址会变成这样-> https://www.miaodongketang.cn/?loginName=asdad&pwd=asdasd  -->
		<form action="https://www.miaodongketang.cn">
			<table border="1px" cellspacing="0" width="600px" >
				<tbody>
					<tr  height="40px">
						<td rowspan="4" align="center" style="color: red;" >总体信息</td>  <!-- 合并一列中的四行-->
						<td colspan="2"></td>  <!-- 合并一行中的两列-->
					</tr>
					<tr height="40px"  >
						<td width="140px" align="right">用户名:</td>
						<td> <input type="text"  value="初始值" name="loginName"/> </td>
					</tr>
					<tr height="40px"> 
						<td width="140px" align="right">密码:</td>
						<td> <input type="password" name="pwd" /> </td>
					</tr>
					<tr height="40px">
						<td colspan="2" align="center"> 
							<input type="submit" value="提交" style="width: 80px; height: 30px; background-color: #E06C75 ;" />
							<input type="reset" value="重置" />
						</td>
					</tr>
				</tbody>
			</table>
		</form>
	</body>
</html>
```

<img src="image/提交表单案例.png" alt="提交表单案例" style="zoom:50%;" />





### get请求和post请求,提交数据和获取数据的表单补充内容

- **提交隐秘数据叫 `post` 请求,  提交普通数据叫 `get` 请求**
    - **两者的区别:**
        - get 请求通常表示获取数据
        - post 请求通常表示提交数据
        - get  请求发送的数据都写在地址栏上
        - post 请求发送的数据用户不可见.
        - **get请求不能提交大量数据, 但post可以, 因此不要混用**

```html
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
        <!-- method="get" 点击提交后网址的数据 https://www.baidu.com/?login=asd&pass=pwd -->
        <!-- method="post" 点击提交后网址的数据  https://www.baidu.com/search/error.html -->
		<form action="http://www.baidu.com" method="get" >
			<p>
				<input type="text" name="login" value="asd" />
			</p>
			<p>
				<input type="password" name="pass" value="pwd" />
			</p>
			<p>
				<input type="submit" />
			</p>
		</form>
	</body>
</html>
```

<img src="image/get请求和post请求.png" style="zoom:50%;" />



## span容器和div容器标签

- **span,  一个容器标签,不具备任何特殊功能, 仅当作容器来使用**
    - **用于包裹一段文本, 便于给文本增加样式**
        - **容器相当于是个隐形方框, 它包裹了写入的文本, 并且在这个防框内修改文本**
- **容器默认是看不见的**



- **div 一个通用容器标签, 不具备任何特殊功能, 仅当作容器来使用. 可以包裹任何内容,也可以包裹容器**
    - **甚至两个容器还可以发生重叠和覆盖**
- **容器特点:**
    - **空的div, 默认宽度 100%, 高度为0**
        - 当添加内容时, 容器的高度才会被撑开
- **属性 `height` 设置的是 div容器的高度**
    - **属性 `line-height` 设置的是 容器内的 行高, 如果将这两个值设置成相等, 那么文字会自动垂直居中**
- 

```html
<span style="text-align:center; margin:auto; background-color:gray; font-size:24px; color:white; "> 文本 </span>

<!-- text-align:center; 让内部元素(文本)水平居中,  margin:auto; 让元素(容器)本身水平居中 -->
<!-- color:white;  设置文字颜色background-color: gray; 设置背景颜色  -->
<!-- font-size:24xp; 设置字体大小 -->




<!-------------------- 显示效果 ------------------------------------------->
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<!-- 使用div来包裹容器,设置容器距离两边的宽度为自动 会自动居中margin: auto,
		      左右两边的宽度 width: 500px, 以及容器的最小宽度-->
		<!-- 当设置容器的最小宽度  width之后, 网页缩小就不能小于这个宽度了-->
		<div style="color: #5c5e62; margin: auto; width: 500px;"> 
		
		<!-- 将深海简介 居中 -->
		<p align="center">
			<!-- 然后 针对 文本进行设置.并不作用于位置关系 , 背景颜色是灰色gray, 字体白色, 字号24像素 -->
			<span style=" background-color: gray; color: white; font-size: 24px;">
				 深海简介
			</span>
		</p>
		
		<p>
			 <strong>那么我看的时候应该是十岁出头，看到一半</strong>
		    <span style="color: darkgreen;">(那个人脑袋里长出的东西布满了整个墙）之后直接扯着我妈尖叫想带着饮料回家我妈：</span>
			？不是很恐怖啊
		 </p>
		 
		<p>
			<strong>然后结尾女主见到了那个骷髅和那个镜像一样的东西时 我直接升天了（小时候对骷髅骨头尸体这种怕到死）</strong>
		</p>
		<p>
			<span style="color: #f6a829;">买张电影票 你买不了吃亏 买不了上当我妈我妈：？不是很恐怖啊我妈：？不是很恐怖啊：</span>
			<strong>买张电影票 你买不了吃亏 买不了上当我妈我妈：</strong>
			？不是很恐怖啊我妈：？不是很恐怖啊：
			买张电影票 你买不了吃亏 买不了上当我妈我妈：
			<strong>？不是很恐怖啊我妈：？不是很恐怖啊：</strong>
		</p>
		</div>
	</body>
</html>
```

<img src="image/dev和span容器.png" style="zoom:50%;" />























