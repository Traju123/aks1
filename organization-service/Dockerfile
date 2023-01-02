FROM maven:3.8.6-openjdk-18-slim
COPY . .
RUN mvn clean install -DskipTests
EXPOSE 8081
ENTRYPOINT ["sh", "-c"]
CMD ["exec java -jar /target/organization-service-1.2.jar"]

