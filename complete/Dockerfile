FROM java:7 

# Install maven
RUN apt-get update
RUN apt-get install -y wget git-core maven

WORKDIR /ecs-demo-rest-api

# Prepare by downloading dependencies
ADD pom.xml /ecs-demo-rest-api/complete/pom.xml

# Adding source, compile and package into a fat jar
#ADD src /ecs-demo-rest-api/complete/src
#RUN ["mvn", "package"]

EXPOSE 9000
CMD ["mvn", "spring-boot:run"]
