# INTERVIEW QUESTIONs


### 1. What is REST API? ITS characteristics and role?

*rest api is a way for different systems(Frontend->backend) to communicate over HTTP using standard methods  like GET,POST,PUT,DELETE.*


Key Characteristics 
- stateless
- client server archi
- uniform interface
- cacheable
---
### 2. Difference between PUT and POST?

###### *POST* : Used to create a new resource
###### *PUT* : Used to update or replace  an existing resource.

###### Based on idempotency?
- IT means same request same result

- PUT = idempotent ✅
- POST = not idempotent ❌
---
### 3.Request Body vs Request Parameters

***Request Body***
- *Data sent inside the HTTP request* 
- *used in POST,PUT,PATCH*

***Request Parameters***
- *Data sent inside parameters*
- Part of url
---
### 4. What is document in mongoDB?

*A document  is a record stored in a collection*
- It is stored in BSON format
- Similar to json
---
### 5. Difference between Embedding vs Reference in MONGODB

- Embedding is nested documents.
- Store related data inside the same document

**While referencing stores in seperate collection and link using IDs**

---
### 6. What is objectId  in mongoDB?

An object id is a special data type used as the default value for the _id field in every document.

- it acts as unique identifier of each document
- automatically generated if not provided

---
### 7. What is Tag in HTML?

- In HTML its the basic building block used to define elements on a web page.
- Tags tell how to display content
- Tags are written inside angular brackets `<>`

---
### 8. What is a HYPERLINK

- A hyperlink is a clickable element that takes you to another page, file or location.
- its created using anchor tags

Types of hyperlink
- internal 
- external
- open in  new tab

---
### 9. What is virtual dom how it helps in react render

In React, the **Virtual DOM (VDOM)** is a lightweight copy of the real DOM stored in memory

How it works:

1. React creates a **virtual DOM tree**
2. When state/props change → React creates a **new VDOM**
3. It compares old vs new VDOM (**diffing**)
4. Updates only the changed parts in the **real DOM**

---

### 10. What is use state what it returns and how it helps in render

its a react hook which manages state in functional component

**It return 
current value
set state to update the value

***How it helps in rendering:***
    1. Updates the state
    2. Triggers a **re-render**
    3. Updates only the changed UI (using Virtual DOM)
    
---
### 11.What is event loops in node.js

*This is an core mechanism that allows node.js to handle asynchronous operation using a single thread.*

- JavaScript is **single-threaded**, meaning it executes one task at a time.  
But Node.js can still handle thousands of requests because of the **event loop + async system**.

---
### 12.What is nodejs asynchronous behaviour?

It means task of `API calls, reading files, database` does not block execution.

- its non blocking I/O

----
### 13.Difference Between Node.js and JavaScript

**Javascript is a programming language while node.js is an run time enviroment**

**Js runs in browser
**While node.js runs outside of browser

----
### 14.Create nodejs server using node.js inbuilt modules


```node
const http = require("http");

// create server
const server = http.createServer((req, res) => {
  res.writeHead(200, { "Content-Type": "text/plain" });
  res.end("Hello World from Node.js server");
});

// listen on port
server.listen(3000, () => {
  console.log("Server running on http://localhost:3000");
});
```
---

### 15.What is difference between require and import in node?

* `require` is the CommonJS module system used mainly in Node.js and works synchronously at runtime, while `import` is the ES Module system that is statically analyzed before execution, enabling optimizations like tree shaking and better async loading.*
---
### 16.What are endpoints according to rest api?

**An endpoint is a specific URL in a REST API used to access or manipulate resources using HTTP methods.**

---
### 17.What does Statelessness mean according to REST API?

**statelessness in REST means each request is independent and contains all the required information because the server does not store client session state between requests.**

---
