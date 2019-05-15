The demo shows how to generate static docs (HTML5 and PDF) with the swagger2markup-gradle-plugin 
and serve them in a Spring Boot app under http://localhost:9080/docs/index.html 
and http://localhost:9080/docs/index.pdf.
生成swagger离线文档，解决pdf中文乱码问题

1、 修改POM文件swagger.input属性值为本地swagger.json所在路径

2、使用maven命令生成hmtl pdf 文档
   mvn clean test
   
3、注意需要把asciidoctorj-pdf-1.5.0-alpha-zh.16.jar手动添加到本地仓库中去，否则mvn test会失败