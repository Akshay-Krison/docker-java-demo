FROM tomcat:8-jre11
#remove the basic application already exsiting 
RUN rm -rf /usr/local/tomcat/webapps/*
#Copy the var file in to the conatiner root directory
COPY target/varprofile-v2.war /usr/local/tomcat/webapps/ROOT.war
#set container port
EXPOSE 8080
#set command to start the application
CMD ["catalina.sh", "run"]

WORKDIR /usr/local/tomcat/

VOLUME /usr/local/tomcat/webapps