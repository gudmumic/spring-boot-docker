FROM openjdk:11.0.14-jdk

VOLUME /tmp
ADD maven/${project.name}-${project.version}.jar myapp.jar
RUN sh -c 'touch /myapp.jar'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/myapp.jar"]
