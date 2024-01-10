## 目录

- [javaScript高层定义](#javaScript高层定义)
- [js监听器](#js监听器)
  - [async和defer属性](#async和defer属性)
  - [事件监听器](#事件监听器)
- [循环](#循环)


# javaScript高层定义
```html
    <p>Player 1: Chris</p>
    <!-- 这个脚本一定要在 p 标签之后加载 -->
    <script src="./script.js"></script>
```
```css
p {
  font-family: "helvetica neue", helvetica, sans-serif;  /* 设置了字体系列，按照给定的顺序，首选字体为 “helvetica neue”，如果该字体不可用，则选择 helvetica，最后备用的字体为 sans-serif。 */
  letter-spacing: 1px;  /* 设置字母间距为 1 像素。 */
  text-transform: uppercase;    /* 转换文本为大写字母。 */
  text-align: center;           /* 设置文本居中对齐。 */
  border: 2px solid rgb(0 0 200 / 0.6);   /* 设置一个 2 像素宽的实线边框，颜色为透明度为 0.6 的蓝色（RGB 值为 0、0、200）*/
  background: rgb(0 0 200 / 0.6);     /* 设置背景颜色为透明度为 0.6 的蓝色。 */
  color: rgb(255 255 255 / 1);        /*  设置文本颜色为完全不透明的白色。 */
  box-shadow: 1px 1px 2px rgb(0 0 200 / 0.4);   /* 添加一个 1 像素偏移的 2 像素模糊的阴影效果，颜色为透明度为 0.4 的蓝色。 */
  border-radius: 10px;      /* 设置边框的圆角半径为 10 像素。 */
  padding: 3px 10px;        /* 设置内边距为上下各 3 像素，左右各 10 像素。  */
  display: inline-block;    /* 将元素设置为内联块元素，使其在一行中显示，并具有块级元素的盒模型特性。 */
  cursor: pointer;          /* 将光标样式设置为指针样式，表示该元素可点击。 */
}

```

```javascript
const para = document.querySelector("p");  // 通过 querySelectorAll() 函数，可以选择页面上的所有按钮
console.info(para); // 输入log
// 使用 addEventListener() 为每个按钮分配一个处理器
para.addEventListener("click", updateName);  // 用一个 click 事件来检测按钮什么时候被点击，然后运行代码更新文本标签。

function updateName(el) {
  const name = prompt("Enter a new name");
  para.textContent = `Player 1: ${name}`;
}
```
![javaScript高层定义](./assets/javaScript高层定义.png)

# js监听器
```javascript
// 这是一个事件监听器，它监听浏览器的 DOMContentLoaded 事件，其标志了 HTML 文档体完全加载和解析。
// 该代码块中的 JavaScript 在事件被触发后才会运行，因此避免了错误
document.addEventListener("DOMContentLoaded", () => {
  // …
});
```

## async和defer属性
脚本阻塞问题实际有两种解决方案——async 和 defer
- async
  - 浏览器遇到 async 脚本时不会阻塞页面渲染，而是直接下载然后运行。但是，一旦下载完成，脚本就会执行，从而阻止页面渲染。脚本的运行次序无法控制
- defer
  - 使用 defer 属性加载的脚本将按照它们在页面上出现的顺序加载。在页面内容全部加载完毕之前，脚本不会运行，如果脚本依赖于 DOM 的存在（例如，脚本修改了页面上的一个或多个元素），这一点非常有用。
```html
// async 属性
<script async src="js/vendor/jquery.js"></script>

// defer 属性
<script defer src="js/script2.js"></script>
```

## 事件监听器
侦听事件发生的结构称为事件监听器（Event Listener），响应事件触发而运行的代码块被称为事件处理器（Event Handler）。
```html
<input type="submit" value="Submit guess" class="guessSubmit" />
```
```javascript
// 下面的代码表示，当点击在页面上的一个  Submit guess 按钮后，就会触发 checkGuess 函数，并弹出一个窗口。

// 找到文档中具有 guessSubmit 类名的元素，并将其存储在变量 guessSubmit 中。
const guessSubmit = document.querySelector(".guessSubmit"); 
// 为找到的元素添加了一个点击事件监听器，当用户点击该元素时(就是发生click事件)，会调用 checkGuess 函数。
guessSubmit.addEventListener("click", checkGuess);
function checkGuess() {
  // 弹出一个告警窗口，显示 I am a placeholder
  alert("I am a placeholder");
}
```

## 循环
```javascript
// 这段代码通过 querySelectorAll() 方法创建了一个包含 <div class="resultParas"> 内所有段落<p>的变量，
// 然后通过循环迭代，删除每个段落的文本内容。
// 即使 resetParas 是一个常量，我们也可以更改其内部属性，例如 textContent。
const resetParas = document.querySelectorAll(".resultParas p");
for (const resetPara of resetParas) {
  resetPara.textContent = "";
}
```


