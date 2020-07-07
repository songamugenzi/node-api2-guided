# Node API 2 Guided Project Starter Code

Guided project starter code for **Node API 2** module.

In this project we will learn how to create a very simple Web API using `Node.js` and `Express`, and cover how to use `Express Routers` to break up the application to make it more maintainable.

## Prerequisites

-   a REST client like [insomnia](https://insomnia.rest/download/) or [Postman](https://www.getpostman.com/downloads/) installed.

## Project Setup

-   [ ] fork and clone this repository.
-   [ ] **CD into the folder** where you cloned **your fork**.
-   [ ] type `npm i` to download dependencies.

Please follow along as the instructor builds the API step by step.

| Action           | Non RESTful way | RESTful Design |
| :--------------- | :-------------- | :------------- |
| Add a client     | /newclient      | POST /clients  |
| List all clients | /clientlist     | GET /clients   |

Organizing API Files

-   by type
    -   /routers
        -   clientsRouter.js
        -   profilesRouter.js
    -   /models
    -   /tests
        -   clients.test.js
        -   profiles.test.js
-   by feature/resource
    -   /clients
        -   client.router.js
        -   client.model.js
        -   client.test.js
    -   /vehicles
    -   /profiles
-   hybrid
    -   components
        -   Users
            -   UserList.js
            -   UserDetails.js
            -   NewUser.js
    -   Users
        -   reducers
        -   actionCreators
        -   components

## Query String

https://www.google.com
/search
? --> marks the beginning of the query string
source=hp ---> key/value pair
& ---> separates key/value pairs
ei=tacEX4fHOs64-gTb0q_ACg
&
q=mdn+query+string
&
oq=mdn+query+string

```js
req.query = {
    source: "hp",
    ei: "tacEX4fHOs64-gTb0q_ACg",
    q: "mdn+query+string",
};
```

## Sub Routes

Chat

-   org

    -   channels
        -   messages
            -   reactions --> emoji

-   /orgs CRUD
-   /channels { orgid: 1, ...channelData }, POST, GET /orgs/23/channels; DELETE /channels/23
-   /messages
-   /reactions ->>>> sub route candidate, it does not make sense outside of a message.
-   /emojis

