# chinaaddress
地址库文件（利用网页get到的数据截取，木有办法，不会服务器，不知道怎么玩）
亲测好用。

##使用方法：
>1、get请求，请求地址：https://github.com/gudujiucheng/chinaaddress/releases/tag/1.0
>2、请求返回的串是一个网页需要截取
>截取方法
***
int end = response.indexOf("自己右键看源码找结束位置");
***
int start = response.indexOf("开始位置");
***
response = response.substring(start+s.length(),end)+"}";
***
然后解析加入到数据库直接用就行了
