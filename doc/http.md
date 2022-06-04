# bookget
bookget 数字图书馆下载工具

#### 通用批量下载(http/https链接)
因考虑到bookget不可能支持无穷数量的网站，特别提供通用批量下载功能。当然，这个功能在很多下载工具中都有了，bookget只是提供自动生成 0001/0002这样的顺序下载，以保证批量下载时文件名不乱。

#### 使用方法：
启用此功能，需要在config.ini中找到 AutoDetect = 0 改为 1，保存文件。

```
AutoDetect = 1
```
设置为1以后，就关闭了内置支持的二十多个图书馆。用完以后，不要忘记再改为0。

例如：
第1页网址是  
```
https://lbezone.ust.hk/obj/6/o/b1129168/ebook/pg00001.jpg
```
第2页网址是  
```
https://lbezone.ust.hk/obj/6/o/b1129168/ebook/pg00002.jpg
```
……
第84页网址是    
```
https://lbezone.ust.hk/obj/6/o/b1129168/ebook/pg00084.jpg
```
那么，你可以在【urls.txt】文件中填写以下URL，即可下载全部84页。
```
https://lbezone.ust.hk/obj/6/o/b1129168/ebook/pg000(01-84).jpg
```
注解：支持(01-100) 、(1-100)、(001-100)等格式通配符写法。

如果你想下载第31-40页，可以使用以下URL
```
https://lbezone.ust.hk/obj/6/o/b1129168/ebook/pg000(31-40).jpg
```
如果你只想下载第1页，可以使用以下URL：
```
https://lbezone.ust.hk/obj/6/o/b1129168/ebook/pg00001.jpg
```
