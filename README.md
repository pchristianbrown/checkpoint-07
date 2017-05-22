# Week 10

## Mongoose

### Question #1

Describe the differences between a SQL and NoSQL database, and when you might use each.

```text
SQL is a static relational database that uses predetermined schemas/tables to organize the information while NoSQL is a dynamic database that uses documents to organize information using key-value pairs to sort the information. SQL is used for more complex and scalable applications whereas NoSQL can be used in more "On the fly" situations.
```

### Question #2

What's wrong with this Mongoose code and how might we fix it?

```js
var results = AuthorModel.find({name: "Bob"});
console.log(results);
```

> Hint: Assuming there is a document with a name of "Bob", why does `results` not contain an author model on the second line?

```js
****var mongoose = require('mongoose')
****mongoose.connect('mongodb:localhost/AuthorModel')
```

### Question #3

Convert the Ruby and ActiveRecord code below into Javascript and Mongoose code:

```rb
@andy = Instructor.find_by(name: "Andy")
@andy.wishlist_items.create(description: "Resin Laying Deer Figurine, Gold")
```

```js
var Instructor = mongoose.Instructor;
var wishlist_items =
```

### Question #4

Convert the following create method in Mongoose to ActiveRecord.

```js
var author = new Author({name: req.body.name})
author.save(function(err){
  if (!err){
    res.redirect("authors")
  }
})
```

```rb
# Your answer...
```

## Express

### Question #5

What is module.exports and why do we use it?

```text
It allows you to move or export code from one file to another.
```

### Question #6

Write one Express route for each of the four HTTP methods.

Then, make each route respond with a one-word string containing the RESTful action that would most likely be associated with this route.

```js
var express = require("express");
var app = express();

// Your code starts here...

```

### Question #7

Describe the differences between Express and Rails as backend frameworks.

```text
Express is used as a Javascript framework whereas Rails is used as a Ruby backend framework.
```

### Question #8

What do the following lines of code do?

```js
var bodyParser = require("body-parser")
app.use(bodyParser.json())
app.use(bodyParser.urlencoded({extended: true}))
```

```text
Line 97 references the use of the code 'body-parser'. Line 98 returns the 'body-parser' back in a json format. Line 99 allow the code to be viewed in html.
```

### If You Finish Early...

Take a look at these [front end developer interview questions](https://github.com/h5bp/Front-end-Developer-Interview-Questions/blob/master/README.md)
