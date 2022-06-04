# bookget
bookget 数字图书馆下载工具

#### 支持的数字图书馆URL格式：

在urls.txt文件中，毎行一个URL，回车换行，可以有多个URL。
原则上，以你能在浏览器中【在线阅读】书籍正文的URL为下载地址。

+ 中国国家图书馆：
```
整书多册URL：http://read.nlc.cn/allSearch/searchDetail?searchType=1002&showType=1&indexName=data_892&fid=411999021002
或者单册URL：http://read.nlc.cn/OutOpenBook/OpenObjectBook?aid=403&bid=70621.0
```


+ hathitrust 数字图书馆-图书单册URL 

```
https://babel.hathitrust.org/cgi/pt?id=uc1.c087423515&view=1up&seq=1&skin=2021
```


+ 哈佛大学图书馆-图书在线阅读（分享）URL
```
https://iiif.lib.harvard.edu/manifests/view/drs:53262215
```


+ 日本京东大学图书馆-图书在线阅读URL
```
https://rmda.kulib.kyoto-u.ac.jp/item/rb00024956
```


+ 日本京都大学人文科学研究所-图书在线阅读URL
```
http://kanji.zinbun.kyoto-u.ac.jp/db-machine/toho/ShiSanJingZhuShu/html/A002menu.html
```


+ 美国国会图书馆 – （大陆需自备海外VPN，免VPN方法在后文批量文件下载有提及。）
```
https://www.loc.gov/item/2014514163/
```


+ 普林斯顿大学图书馆 – 图书在线阅读URL
```
https://catalog.princeton.edu/catalog/9940468523506421
https://dpul.princeton.edu/catalog/99915a8b423b596e47540e3feeee19b8
```


+ 日本国立国会图书馆 – 部分图书在线阅读URL（其它的可以手动打印下载）
```
https://dl.ndl.go.jp/info:ndljp/pid/8929985
```


+ 中国台北图书馆古典与特藏文献 –（白天很慢，可夜间或清晨下载）
```
https://rbook.ncl.edu.tw/NCLSearch/Search/SearchDetail?item=422a7598bd0046aebf2684ae0f945d25fDcyODIz0&image=1&page=&whereString=&sourceWhereString=&SourceID=
```


+ 日本E国宝 – 画册在线阅读URL（部分单图有误，暂未修复）
```
https://emuseum.nich.go.jp/detail?content_base_id=100168&content_part_id=009&langId=zh&webView=
```


+ 日本宫内厅书陵部 – 图书在线阅读URL
```
https://db2.sido.keio.ac.jp/kanseki/T_bib_frame.php?id=006754
```


+ 日本东京大学东洋文化研究所 汉籍善本 – 图书在线阅读URL   
```
http://shanben.ioc.u-tokyo.ac.jp/main_p.php?nu=C5613401&order=rn_no&no=00870
```


+ 中国香港中文大学图书馆 – 图书在线阅读URL（需自备VPN，从海外访问）
```
https://repository.lib.cuhk.edu.hk/sc/item/cuhk-412225#page/1/mode/2up
```


+ 牛津大学博德利图书馆 – 图书在线阅读URL
```
https://digital.bodleian.ox.ac.uk/objects/310cb04e-6bce-44e3-85b5-03417c9644a8/
```


+ 日本国立公文书馆（内库文库） - 图书在线阅读URL
```
https://www.digital.archives.go.jp/DAS/meta/listPhoto?LANG=default&BID=F1000000000000095447&ID=&NO=&TYPE=
```


+ 日本早稻田大学图书馆 – 图书在线阅读URL
```
https://archive.wul.waseda.ac.jp/kosho/ri08/ri08_01899/
```


+ 日本东洋文库（丝绸之路项目） - 图书在线阅读URL
```
http://dsr.nii.ac.jp/toyobunko/XI-6-A-16/V-1/
```


+ 韩国国家图书馆 （特殊情况，详见独立PDF说明文档）
```
http://lod.nl.go.kr/page/CNTS-00076977176
```


+ 新日本古典籍综合数据库（详见独立PDF说明文档）
```
https://kotenseki.nijl.ac.jp/biblio/100270332/viewer/1
https://kotenseki.nijl.ac.jp/biblio/100270332
```


+ 德国柏林图书馆URL
```
https://digital.staatsbibliothek-berlin.de/werkansicht?PPN=PPN3343671770
https://digital.staatsbibliothek-berlin.de/werkansicht?PPN=PPN3343671770&PHYSID=PHYS_0001
```

+ 英国图书馆URL（只生成dezoomify-rs.urls文件，生成后，请双击它下载）
```
http://www.bl.uk/manuscripts/Viewer.aspx?ref=or_6814!1_fs001r
```

+ 中国香港科技大学图书馆URL
```
https://lbezone.ust.hk/bib/b1129168
```

+ 中国台北故宫博物院-善本古籍URL （详见独立PDF说明文档）

+ 日本国立历史民俗博物馆
```
单册URL:
https://khirin-a.rekihaku.ac.jp/sohanshiki/h-172-1
https://khirin-a.rekihaku.ac.jp/sohanshiki/h-173-1

多册URL，使用和“批量下载”相同格式，但是无需修改config.ini中配置。
如：第1-9册，第10-90册。用圆括号包围数字。   

https://khirin-a.rekihaku.ac.jp/sohanshiki/h-172-(1-90)
https://khirin-a.rekihaku.ac.jp/sohankanjo/h-173-(1-61)
```

+ 日本本市立米泽图书馆
```
https://www.library.yonezawa.yamagata.jp/dg/AA001_view.html
https://www.library.yonezawa.yamagata.jp/dg/AA002_view.html
```

+ 日本庆应义塾大学图书馆
```
https://dcollections.lib.keio.ac.jp/ja/kanseki/110x-24-1
```

+ 日本关西大学图书馆
```
https://www.iiif.ku-orcas.kansai-u.ac.jp/books/210185040#?page=1
```

+ 中国河南省洛阳市图书馆   
```
http://221.13.137.120:8090/productshow.php?cid=4&id=112
```
+ 中国浙江省温州市图书馆 - 瓯越记忆(自动下载相关资源分卷分册)   
```
https://oyjy.wzlib.cn/resource/?id=61e4cff7727da20473b3ed89
https://oyjy.wzlib.cn/resource/?id=61e4c764505415b2e6921e5e
```
+ 巴伐利亚州立图书馆
```
https://ostasien.digitale-sammlungen.de/view/bsb11129280/1
```
+ 斯坦福大学图书馆
```
https://searchworks.stanford.edu/view/4182111   
```
+ 中国广东省深圳市图书馆-古籍
```
https://yun.szlib.org.cn/stgj2021/srchshowbook?type=4&book_id=18269  
https://yun.szlib.org.cn/stgj2021/srchshowbook?type=1&book_id=18017
```