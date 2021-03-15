## DOM型XSS、反射型、存储型XSS
DOM型XSS是由于浏览器解析特性导致的漏洞，无需与服务器交互，而反射型、存储型XSS都需要服务器参与


## JSONP
JsonP（由于返回JSon格式数据，故称JSON Padding）是一种跨域获取数据的方法，利用了script标签没有跨域限制的特性来达到跟第三方通讯的目的。

可以跨域的标签有：script、img、vedio、audio、embed、frame、iframe、link、applet、object

主域一致的站点，若端口、协议相同，可设置document.domain来进行通讯。

let xmlhttp = new XMLHttpRequest();
xmlhttp.open("post", "url", true);// true = async
xmlhttp.setRequestHeader("Content-type","application/x-www-form-urlencoded");
xmlttp.send(data);


