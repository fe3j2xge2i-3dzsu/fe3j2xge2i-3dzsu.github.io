---
layout: default
---

<script src="https://cdnjs.cloudflare.com/ajax/libs/js-sha256/0.9.0/sha256.min.js"></script>
<script type="text/javascript">   
function password() {
    var testV = 1;   
    var pass1 = prompt('请输入密码',''); // 不知道如何在 GitHub Pages 里面使用过hash函数
    var passHash = sha256(pass1);
    var correctHash = 'f158f6ea58c1045f47549b54b65d25a283c35f28e4ae9c671a6950387c7c5d97';
    while (testV <= 3) {   
        if (!pass1)   
            window.location.href = "https://www.google.com";  // 跳转到指定页面 
        if (passHash == correctHash) { // 初始密码
            alert('密码正确');   
            document.getElementById('protected-content').style.display = 'block'; // 密码正确时显示页面内容
            return;   
        }   
        testV += 1;   
        var pass1 = prompt('密码错误!请重新输入:');   
    }
    alert('错误次数过多，将跳转到其他页面。');
    window.location.href = "https://www.google.com";  // 跳转到指定页面
}

window.onload = password; // 页面加载后调用password函数
</script>

<!-- 页面内容默认隐藏 -->
<div id="protected-content" markdown="1" style="display: none;">

# Qi-Group (Shanghai AI Lab)

<p align="center">
    🏠 <a href="https://github.com/unsosp1ro/unsosp1ro.github.io">Home Page</a>  |   🤗 <a href="https://github.com/unsosp1ro/unsosp1ro.github.io">Model</a>  |   📊 <a href="https://github.com/unsosp1ro/unsosp1ro.github.io">Dataset</a>  |   📄 <a href="https://github.com/unsosp1ro/unsosp1ro.github.io">Paper</a> 
</p>


## TODO 
分页维护
每个方向一页
每个具体研究内容的更新
每个方向都有自己的paper list和最新进展

## About

You can edit this page using Markdown syntax.

## 通专融合基础模型架构设计

| 具体方法 | 方向1 | 方向2 | 方向... |
| :------: | :---: | :---: | :-----: |
|  方法1   | Text  | Text  |  Text   |
|  方法2   | Text  | Text  |  Text   |


## 群体智能系统与关键技术研究

| 具体方法 | 方向1 | 方向2 | 方向... |
| :------: | :---: | :---: | :-----: |
|  方法1   | Text  | Text  |  Text   |
|  方法2   | Text  | Text  |  Text   |

## 科学智能与具生智能应用

| 具体方法 | 方向1 | 方向2 | 方向... |
| :------: | :---: | :---: | :-----: |
|  方法1   | Text  | Text  |  Text   |
|  方法2   | Text  | Text  |  Text   |

</div> <!-- 结束 protected-content div -->
