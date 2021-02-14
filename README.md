# About this Spring boot application

### Notes
* Download spring boot application from start.spring.io
* Add @EnableAutoConfiguration to Application.java file (in our case DemoApplication.java)
* Create another controller class (in our case Welcome.java)
* Create index.html file under resource/static folder
* Create a method in controller class and map it to index.html file

##GCLOUD
### Install gcloud

```
brew install --cask google-cloud-sdk

source '/usr/local/Caskroom/google-cloud-sdk/latest/google-cloud-sdk/completion.zsh.inc'
source '/usr/local/Caskroom/google-cloud-sdk/latest/google-cloud-sdk/path.zsh.inc'
```


### Configure gcloud
 * Execute the command ```gcloud init```
 * Login to your account (if not already logged in)
 * choose project to deploy


### publish to selected gcloud application
 * Execute the following command to publish to selected gcloud application
```
 ./mvnw -DskipTests package appengine:deploy
```

## Understandings
* Whatever we kept under resource/static folders will be added to the web application automatically
* If there is any index.html inside resource/static folder, then it will be considered as welcome page the application automatically
* In pom.xml, packaging type should be jar (Otherwise, I faced an issue "Project stopped with exit status 0")