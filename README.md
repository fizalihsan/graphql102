# GraphQL - Java implementation


This is the source code for the "Getting started with GraphQL Java and Spring Boot" which 
is available here: https://www.graphql-java.com/tutorials/getting-started-with-spring-boot/ 

```bash
# build and run Spring Boot app which publishes the API
gradle clean build bootRun

# install GraphQL playground
brew cask install graphql-playground

# open GraphQL playground and enter http://localhost:8080/graphql/

# curl version
curl 'http://localhost:8080/graphql' -H 'Accept-Encoding: gzip, deflate, br' -H 'Content-Type: application/json' -H 'Accept: application/json' -H 'Connection: keep-alive' -H 'DNT: 1' -H 'Origin: file://' --data-binary '{"query":"# Write your query or mutation here\n{\n  bookById(id: \"book-1\") {\n    id\n    name\n    pageCount\n    author {\n      firstName\n      lastName\n    }\n  }\n}\n"}' --compressed
```