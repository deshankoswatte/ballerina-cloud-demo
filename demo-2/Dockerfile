FROM ballerina/ballerina:1.0.5
WORKDIR /home/sample
COPY hello_service.bal /home/sample/
RUN ballerina build hello_service.bal

FROM openjdk:8-jre-alpine
WORKDIR /home/ballerina
COPY --from=0 /home/sample/hello_service.jar .
EXPOSE  9090
CMD java -jar hello_service.jar