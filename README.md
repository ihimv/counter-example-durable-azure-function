# counter-example-durable-azure-function
## Creating a counter using Durable Entities in Durable Azure Function

It is possible to persist the state of an entity in Durable Azure Function. This state is not lost even when the function restarts and can be accessed accross instances of Azure Function, regardless of on which server the function runs.

### The Counter Example  has 3 REST APIs 
1.    **increment**: [GET,POST] http://localhost:7071/api/increment
2.    **decrement**: [GET,POST] http://localhost:7071/api/decrement
3.    **getCounter**: [GET] http://localhost:7071/api/getCounter


### Running the Counter Example 
To run the example, the Azure Storage Emulator has to installed locally. 
1.    Build and run the example.
2.    Call the _increment_ API multiple times from the browser itself.
3.    Call the _getCounter_ API to see the current value of the counter.
4.    Stop the Counter Example Azure Function 
5.    Run the Azure Function again
6.    Check the last value of the counter by calling _getCounter_ API
7.    Our counter value is still the same, as we had before stopping the Azure Function. Cheers!

