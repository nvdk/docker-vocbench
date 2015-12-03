FROM tomcat:7

ADD https://bitbucket.org/art-uniroma2/vocbench/downloads/VOCBENCH_2.3.zip /VOCBENCH.zip
RUN mkdir /vocbench && apt-get update && apt-get install unzip && unzip /VOCBENCH.zip -d /vocbench/ && mv  /vocbench/vocbench-2.3.war /usr/local/tomcat/webapps/vocbench.war
