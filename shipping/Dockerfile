FROM maven:3.5
WORKDIR /app
COPY db
COPY src
COPY pom.xml
ENV  CART_ENDPOINT=cart:8080 \
     DB_HOST=mysql
CMD ["java" , "shipping.jar"]     

    
