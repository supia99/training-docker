# training-docker

## tomcat
- 参考にしたimage：tomcat:8.5-jdk21-openjdk
```
# pwd
/usr/local/tomcat/conf
# ls
Catalina         catalina.properties  jaspic-providers.xml  logging.properties  tomcat-users.xml  web.xml
catalina.policy  context.xml          jaspic-providers.xsd  server.xml          tomcat-users.xsd
```

### command
```
docker run --name tomcat tomcat:8.5-jdk21-openjdk
docker exec -it tomcat /bin/bash
docker build -t original-tomcat:1 .
```