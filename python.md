<center>
    python
    <br>
    pzc
</center>
***

***

## 基础

***

### 字符串

* 字符串前的字母 ：
  - u：字符串包含中文，使用中文编码
  - r： 表示普通字符串，无转义
  - b： bytes字符串，必须是16进制数，或者ASCII字符

***

***

## 扩展

***

### beautifulsoup

[官方文档](https://beautifulsoup.readthedocs.io/zh_CN/v4.4.0/)

* 对象种类：BeautifulSoup将html转换成树形结构，节点的对象类别包括：Tag，NavigableString，BeautifulSoup，Comment

  - Tag：Tag对象与XML或者HTML中tag相同。包含关键字name，attrs，attrs与字典相同

    ```python
    soup = BeautifulSoup('<b class="boldest">Extremely bold</b>')
    tag = soup.b
    type(tag)
    # <class 'bs4.element.Tag'>
    tag.name
    # u'b
    tag.name = "blockquote"
    tag
    # <blockquote class="boldest">Extremely bold</blockquote>
    tag['class']
    # u'boldest'
    tag.attrs
    # {u'class': u'boldest'}
    ```

    

***

### requests

[官方文档](https://requests.readthedocs.io/zh_CN/latest/user/quickstart.html)

* 发送请求：支持GET，POST，PUT，DELETE，HEAD，OPTIONS，返回**Response**类型的对象，包含所有信息
* 传递参数：使用params传递参数，params是一个字符串字典，值为none的键不会被传递，可传递列表
* 解码：返回的text会被自动解码，使用encoding关键字可以改变解码方式
* 定制头请求：使用headers参数，传递dict

***

update 2020.7.1