# chinaaddress
地址库文件，创建一个免费的能返回地址json串的东东

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
