# counter-example-durable-azure-function
## Creating a counter using Durable Entities in Durable Azure Function

It is possible to persist state of entity in Durable Azure Function. The state of the entity is not lost even when the function restarts. This entity can be accessed accross instances of Azure Function, regardless of on which server the function runs.

