# GraphQL Learning Journey


## what is GraphQL: 

GraphQL is a way of asking our server exactly for the data we need and precisely that- no more or no less. Imagine I have a menu (the graphql schema) listing all available dishes (the data). Instead of ordering a set meal (Like REST API), I can order exactly what I want.
The server delivers precisely what I asked for in one request.

Like the below example: Say I just want to know the name of the dish and price,

```
query {
    dish(id: 123) {
        name
        price
    }
}

output

{
    "dish": {
        "name": "Pizza",
        "price": "10.99"
    }
}

```

GraphQL Runtime: The GraphQL runtime is the part of the GraphQL server that handles the execution of the GraphQL query. It takes the query as input and returns the result. The runtime is responsible for parsing the query, validating it against the schema, and executing the query against the data source. The runtime also handles errors and caching. 