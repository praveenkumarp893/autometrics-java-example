# Simple Spring Boot Books API

Basic autometrics integration in spring boot application (https://github.com/LeudiX/Simple-Books-API-with-Spring-Boot)


## Description

A simple API for books management with persistence, basic CRUD operations and security, simple centralized error handling mechanism.

Implementing autometrics from https://github.com/jamsiedaly/autometricsj

## Execution Enviroment

1. Open VSCode
2. Install Java, Maven and Spring packs extensions
3. Reload VScode and configure it for Maven
4. Run (mvn clean install) for dependencies management
5. If no problems, type (mvn sprin-gboot: run) cmd to run the app
6. Open the browser on localhost:8081
7. Enjoy watching my wonderful stuff!!!

### Actions allowed

1. List all books

curl --location 'localhost:8081/api/v1/books'

2. Create a book
curl --location 'localhost:8081/api/v1/books' \
--header 'Content-Type: application/json' \
--data '{
    "title":"Book3",
    "author": "Author3"
}'

3. Delete a book

curl --location --request DELETE 'localhost:8081/api/v1/books/{bookID}'

4. Find a book by title

curl --location 'localhost:8081/api/v1/books/title/{BookTitle}'

### Endpoints

GET localhost:8081/api/v1/books

POST localhost:8081/api/v1/books

