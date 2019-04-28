# servlet
using servlet get current time to show how to write、run and deploy servlet application
Environment:Tomcat8.0+windows system

1:write code
  first of all,you should download a tomcat and make sure you can visit in localhost by default port(8080)
  create a project folder in Tomcat named "project1"
  project1 foler including 3 folders: classes , etc ,src
  description: classes folder was used to save compile class file
               etc folder was used to save web.xml
               src folder was used to save source code
  put Ch1Servlet.java in src folder
  put web.xml in etc folder 
 2：compile
  open cmd 
  enter into your project1 folder
  cpmmand :javac -classpath servlet-api.jar path -d classes Ch1Servlet.java path
  (example:javac -classpath D:\TomCat\lib\servlet-api.jar -d classes D:\TomCat\Project1\src\Ch1Servlet.java)
  then Ch1Servlet.class will be created in  classes folder
3: deploy
  creat a folder in Tomcat webapps folder (save your servlet application file),for example named ServlerProject
  there should be a foler structure ServlerProject folder-WEB-INF folder-classes folder
  put Ch1Servlet.class in classes folder,put web.xml in WEB-INF folder
Last step:
  enter into Tomcat bin foler ,then start startup.bat
  open browser ,input "http://localhost:8080/ServlerProject/Serv1"
  then you can see "Servlet getCurrentTime" page 
