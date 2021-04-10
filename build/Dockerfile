FROM maven:3.6.0-jdk-11-slim
RUN apt update
RUN apt -y install git

RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git /tmp/app/
WORKDIR /tmp/app/
RUN mvn package

RUN cp /tmp/app/target/*.war /usr/local/