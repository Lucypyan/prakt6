FROM ubuntu:latest

RUN apt-get update && apt-get install -y \
x11-apps \
xauth \
openjdk-11-jre\
&& rm -rf /var/lib/apt/lists/*

workdir /newapp

copy calc.jar /newapp/

env DISPLAY=:0

cmd ["java","-jar", "/newapp/calc.jar"]
