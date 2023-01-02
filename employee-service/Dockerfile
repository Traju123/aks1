FROM maven:3.8.6-openjdk-18-slim
COPY . .
RUN mvn clean install -DskipTests
EXPOSE 8080
ENTRYPOINT ["sh", "-c"]
CMD ["exec java -jar /target/employee-service-1.2.jar"]

