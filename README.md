# Description
### V1.0 KISS(Keep It Simple Stupid)


This is an intoductory personal project to have an online to-do list using these technologies:
* front-end: React.js
* backend  : Golang & Gin
* database : MySQL


Why did I choose these technologies?
* React.js is a popular framework 
* Golang is an easy to use backend language with an easy to setup Gin framework for API creation. Java would have had too much overhead and been slower to setup if we wanted to use Dropwizard framework.
* MySQL makes most sense for a very simple ToDoList table with just 2 items: _id and text


Why not other language/framework/no-sql?
* As I mentioned above React.js and Golang are popular frameworks with lots of online support and are easy to setup and beging using. 
* No-sql is a more interesting question. I could use a Document NoSQL db, which is the closest to what makes sense, to hold more than just text e.g. type of item, due date, etc. However, this is more complicated than needed for now. In a future version I'll use it, even if it may not make the most sense, so I will relook into the design of this to make it a fun learning experience.

What is the user experience?
* V1.0 is a single user experience to run locally(future versions will delve into the topic of scaling users, access and maybe even cloud e.g. AWS/Azure/Google Cloud/OCI)
* Drop down for states OPEN, CLOSED, ALL items
* "Create" button for a popup to for adding a new item
* Checklist view. Crossed out text with x'ed out boxes for CLOSED items
* Tap item to open up popup to edit the content.
* Ordered by creation time is descending order to have newest at top. As a user I wouldn't want to have to scroll a huge list of items if I choose to view ALL items as well.

What does data flow look like?
* Gin is a the Golang framework to support API CRUDL calls: Create, Update, Delete, List

Database creation?
* Golang has a MySQL driver for creating if a table if it doesn't already exist interface with our local DB.


# Pre-requisite
Have MySQL, golang and a web browser available.

# Running

In one terminal screen run following commands to run the front end React.js server:
```
cd frontend
npm start
```

In another terminal screen, run the following to start the backend golang server:
```
# TODO
```