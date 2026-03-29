FROM maven:3.5 \
     mysql
WORKDIR /app
COPY db /app/db
COPY src /app/src
COPY pom.xml /app
RUN mvn clean package
ENV  CART_ENDPOINT=cart:8080 \
     DB_HOST=mysql
CMD ["java","-jar","target/shipping-1.0.jar"]     

    
