FROM maven:3.5 
WORKDIR /app
COPY db /app/db
COPY src /app/src
COPY pom.xml /app
RUN mvn clean package
ENV  CART_ENDPOINT=cart:8080 \
     DB_HOST=mysql
FROM mysql     
CMD ["java","-jar","target/shipping-1.0.jar"]     

    
