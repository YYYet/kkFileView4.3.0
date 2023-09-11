1.当url被iframe嵌入时，增加部分文件postmessage通信，监听iframe滚动事件

2.去除4.2.1中处理下载连接时会删除文件流名称

3.为解决excel文件转换时出现文字，样式丢失的情况，将项目升级为4.3.0，使用前端解析excel

4.2023 9 11 解决因系统编码引起的缓存名称url编码后查询不到（gbk url编码 utf8 url编码）
此处修改启动脚本强制使用utf8 
jdk-11.0.2\bin\java -Dfile.encoding=utf-8 -Dspring.config.location=..\config\application.properties -jar kkFileView-4.4.0-SNAPSHOT.jar -> ..\log\kkFileView.log