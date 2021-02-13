# About this Spring boot application

### Notes
* Download spring boot application from start.spring.io
* Add @EnableAutoConfiguration to Application.java file (in our case DemoApplication.java)
* Create another controller class (in our case Welcome.java)
* Create index.html file under resource/static folder
* Create a method in controller class and map it to index.html file

### Understandings
* Whatever we kept under resource/static folders will be added to the web application automatically
* If there is any index.html inside resource/static folder, then it will be considered as welcome page the application automatically
* In pom.xml, packaging type should be jar (Otherwise, I faced an issue "Project stopped with exit status 0")