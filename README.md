# counter-example-durable-azure-function
## Creating a counter using Durable Entities in Durable Azure Function

It is possible to persist the state of an entity in Durable Azure Function. The state of the entity is not lost even when the function restarts and can be accessed accross instances of Azure Function, regardless of on which server the function runs.

The example has 3 REST APIs 
1.    **increment**: [GET,POST] http://localhost:7071/api/increment
2.    **decrement**: [GET,POST] http://localhost:7071/api/decrement
3.    **getCounter**: [GET] http://localhost:7071/api/getCounter

