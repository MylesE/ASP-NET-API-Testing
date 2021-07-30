# Pizza-NET-Example 

https://docs.microsoft.com/en-us/learn/modules/build-web-api-aspnet-core/

Steps to run:
- Navigate to the project folder in terminal
- Build & start web API by typing: dotnet run
- Can connect to the web API by opening up a new terminal and typing: httprepl http://localhost:5000
- run ls to see available endpoints, can cd to desired one (example is the pizza one)
- once in the pizza, can run ls again to see available features that the API provides
- In the pizza example, there are five main requests you can make: Get, Get(id), Post, Put, and Delete
- To stop running the web API you can type exit to get out of the localhost shell, and ctrl+c to stop running 
      the API

Sytax for each request:
- Get: Simply typing in get will list a json of the available pizzas
- Get <id>: Will list the json of the specific id pizza (eg. get 2)
- Post -c "{"name":"XXXX", "isGlutenFree":<true/false>}" will add a new pizza to the list with specified parameters
- Put <id> -c "{"id":<id_here>, "name":"XXXX", "isGlutenFree":true/false}" edits the pizza at the specified id
- Delete <id> will delete the pizza at the specified id
  
Note: will let the user know if there is a misinput (eg. deleting/modifying out of index)
