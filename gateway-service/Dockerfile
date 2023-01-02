FROM maven:3.8.6-openjdk-18-slim
COPY . .
RUN mvn clean install -DskipTests
EXPOSE 8080
#COPY target/$APP_FILE $APP_HOME/
#WORKDIR $APP_HOME
ENTRYPOINT ["sh", "-c"]
CMD ["exec java -jar /target/gateway-service-1.2.jar"]

