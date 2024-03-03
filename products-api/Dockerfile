FROM gradle:8.6.0-jdk11

WORKDIR /app

COPY . .

RUN gradle clean build

CMD ["java", "-jar", "build/libs/products-api-0.0.1.jar"]