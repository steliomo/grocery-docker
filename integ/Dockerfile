FROM openjdk:8-jdk-alpine

LABEL maintainer="steliomo@gmail.com" 

VOLUME [ "/opt/grocery/data" ]

EXPOSE 8080

# Prod
ENTRYPOINT [ "java", "-jar", "/opt/grocery/data/grocery-integ.jar", "--spring.config.location=/opt/grocery/data/application.properties"]

# Dev
#ENTRYPOINT [ "java", "-Djava.security.egd=file:/dev/./urandom", "-Xdebug", "-Xrunjdwp:server=y,transport=dt_socket,address=8000,suspend=n", "-jar", "/opt/grocery/data/grocery-integ.jar", "--spring.config.location=/opt/grocery/data/application.properties" ]