# BOOK API - Spring MVC, MySQL, Hibernate Rest API

Book API demonstrates the RESTful web services using Spring MVC. Book API performs all the CRUD operations. User can create a book, read a single book, update a book and delete a book. To communicate with database we will use Hibernate which is our ORM framework and MySQL is the database to store the records.

## Requirements

1. Java - 1.8.x

2. Maven - 3.3.9

3. MySQL - 5.7.12    

## Steps to Setup

**1. Clone the application**

```bash
git clone https://github.com/dibasbehera7/springmvc-bookapi.git
```

**2. Create Mysql database**

```bash
create database bookdb
```

**3. Change mysql username and password as per your installation**

+ open `src/main/resources/db.properties`

+ change `mysql.user` and `mysql.password` as per your mysql installation

**4. Build and run the app using maven**

```bash
mvn package
```

A new WAR file will be generated at `project/target/bookapi-0.0.1-SNAPSHOT.war`, just copy and deploy to your Tomcat.

The app will start running at <http://localhost:8080/bookapi/>.

## Explore Rest APIs

The app defines following CRUD APIs.

    GET /api/book
    
    POST /api/book
    
    GET /api/book/{bookId}
    
    PUT /api/book/{bookId}
    
    DELETE /api/book/{bookId}

You can test them using postman or any other rest client.

### Postman

## GET - /api/book
![image](https://user-images.githubusercontent.com/24310550/82157450-1f441900-989f-11ea-9a0f-ad78a5b8eea6.png)

## POST - /api/book
![image](https://user-images.githubusercontent.com/24310550/82157501-71853a00-989f-11ea-83f3-b2967526c96d.png)

## GET - /api/book/{bookId}
![image](https://user-images.githubusercontent.com/24310550/82157520-95488000-989f-11ea-9f26-2600372d465d.png)

## PUT - /api/book/{bookId}
![image](https://user-images.githubusercontent.com/24310550/82157557-ccb72c80-989f-11ea-94c1-5ba309c407df.png)

## DELETE - /api/book/{bookId}
![image](https://user-images.githubusercontent.com/24310550/82157579-eeb0af00-989f-11ea-8506-a6e33a880369.png)
