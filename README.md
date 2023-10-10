# graphql

This is an example project using Spring for GraphQL.

## Stack and versions
- Java 17
- SpringBoot 3.1.4

## Running

> ./mvnw spring-boot:run

## Try with GraphiQL Playground

Navigate to [http://localhost:8080/graphiql](http://localhost:8080/graphiql)

Write the query below, and press `play`:

```
query bookDetails {
  bookById(id: "book-2") {
    id
    name
    pageCount
    author {
      id
      firstName
      lastName
    }
  }
}
```
