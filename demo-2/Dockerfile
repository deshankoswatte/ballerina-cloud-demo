FROM ballerina/ballerina:1.0.5
WORKDIR /home/ballerina
COPY hello_service.bal /home/ballerina/
RUN ballerina build hello_service.bal
COPY hello_service.jar /tmp

FROM openjdk:8-jre-alpine
WORKDIR /home/ballerina
COPY --from=0 /tmp/hello_service.jar .
EXPOSE  9090
CMD java -jar hello_service.jar