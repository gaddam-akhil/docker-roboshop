FROM maven:3.5
WORKDIR /app
COPY db /app/db
COPY src /app/src
COPY pom.xml /app
ENV  CART_ENDPOINT=cart:8080 \
     DB_HOST=mysql
CMD ["java" , "shipping-1.0.jar"]     

    
