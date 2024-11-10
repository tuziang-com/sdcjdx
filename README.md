# 山东财经大学继续教育学院刷课脚本


## 脚本

学习网站：山东财经大学继续教育学院: http://sdufe.cep.webtrn.cn/np/#/login

脚本地址：[山东财经大学继续教育学院-刷课脚本][2]

## 教程

浏览器安装篡改猴插件后，打开[脚本安装地址][2]，进入后点击安装脚本，安装完成刷新你的学习网页就可以愉快使用了。

## 联系

注：如果需要代学，可以联系我微信yizhituziang或者QQ2422270452

![微信二维码](https://www.tuziang.com/wx.jpg)

## 更多

关键代码分享：
```

//展开所有章节
var chapter = document.getElementsByClassName("s_chapter")
for (var x =0; x < chapter.length; x++)
{
    chapter[x].click()
}
 
var section = document.getElementsByClassName("s_section")
for (x =0; x < section.length; x++)
{
    section[x].click()
}

setInterval(function () {
    var frame = document.getElementsByClassName('s_wrap main_box')[0].getElementsByTagName("iframe")[0].contentWindow.document;
    //模拟点击下一节，有点递归的感觉。
        if (frame.getElementsByClassName("s_point s_pointerct")[0].getAttribute("completestate") == 1) {
            frame.getElementsByClassName("s_point undo_item_bgc")[2].click()
        } else {
            frame.getElementsByClassName("s_point undo_item_bgc")[3].click()
        }
}, 2000)

```


  [1]: https://microsoftedge.microsoft.com/addons/detail/%E7%AF%A1%E6%94%B9%E7%8C%B4/iikmkjmpaadaobahmlepeloendndfphd?refid=bingshortanswersdownload
  [2]: https://greasyfork.org/zh-CN/scripts/509381-%E5%B1%B1%E4%B8%9C%E8%B4%A2%E7%BB%8F%E5%A4%A7%E5%AD%A6%E7%BB%A7%E7%BB%AD%E6%95%99%E8%82%B2%E5%AD%A6%E9%99%A2%E5%88%B7%E8%AF%BE%E8%84%9A%E6%9C%AC
