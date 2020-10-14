# API's

API's (application program interface) allow applications to access data from other applications or databases.

There are hundreds of thousands of API's out there for all sorts of purposes, from tracking movies, to geolocation data, to videe game leaderboards. These all allow for other applications to use their data.

Typically an API data cycle looks like this:

```
Client ->  API  
   ^        |
   |        v
   API <-  DB
```

Client makes a request to the API, then the API accesses some data, and returns that DATA to the client.

Clients usually will access API through HTTP methods (post, put, get, delete)

[<-- Back](../README.md)
