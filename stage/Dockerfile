FROM zenika/alpine-maven:latest
RUN apk add git
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git
RUN mvn package -f ./boxfuse-sample-java-war-hello/pom.xml
RUN mkdir /apps
RUN cp /boxfuse-sample-java-war-hello/target/hello-1.0.war /apps