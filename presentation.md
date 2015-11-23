# Because I'm API

---

# Application Programming Interface

---

# ?

---

# customers
## ===
# developers

---

> A way to architecture your applications around verbs and resources

---

# Developers
# action verbs on nouns
# Key
# Data

---

# When ?
## to create a public API

---

## Once data model is
# stabilized

---

# Unicorn Example

---

# [Uber](https://developer.uber.com/docs)

---

# [Airbnb](http://all-about-airbnb.com/post/127856658166/airbnb-public-api-coming-soon)

---

# [Palantir](https://www.palantir.com/palantir-gotham/platform/)

---

# [Dropbox](https://www.dropbox.com/developers)

---

# Data is everywhere

---

## I data you, you data me.
## They data us, we data them.

---

![boom](https://cdn-images-2.medium.com/max/2000/1*oZeiXDGKeqZgHlDDdm4szw.jpeg)

> Post-it fridge to phone to-do list

---

# 80 - 20

> an extremely small amount is really used.

---

![small](https://cdn-images-2.medium.com/max/2000/1*-Y5_kjdJBPD4l16N6GJtZw.jpeg)

---

# No Bullshit

---

# It was measured.

---

# Why ?

---

# pre-calculating every decision and spoken word

---

# Sometimes...
### it works
### it’s critical
### it fails

---

# obsesión

---

> Even regular data isn’t exciting enough for us any more, we now need even better data.

---

# Big data

---

## seems hard to explain and understand

> Buzz Word ?

---

# 4V's

---

# Volume

> The amount of data all over the world.

---

![volume](https://cdn-images-2.medium.com/max/2000/1*ZXcqepYO3-keuBzOvV1I1A.jpeg)

---

# Velocity

> Stream of fast-moving data.

---

![velocity](https://cdn-images-2.medium.com/max/2000/1*v7w6N80d4LmRaf-8AxNOyQ.jpeg)

---

# Variety

> Different forms of data.

---

![variety](https://cdn-images-2.medium.com/max/2000/1*I6viCqh13pN9Mln0vL02lg.jpeg)

---

# Veracity

> Ambiguity of data.

---

![veracity](https://cdn-images-2.medium.com/max/2000/1*PPWp8RIjS-tTJZIRTiwVag.jpeg)

---

# 90%

> created in the last two years.

---

# Automation

> (again) 80 - 20

---

### recorded
### reduced
### processed
### analyzed
### coerced

---

# Make me feel beautiful

> collect chaotic data, structure them and deliver it in form of beautiful charts

---

# Some examples

---

### Product visits

![visits](https://i.onthe.io/smngozt0j97b4k0no.e4c1ee32.jpg)

---

### Cart

![cart](https://i.onthe.io/smngozsnu16p30rqg.d82a49f1.jpg)

---

### Lost sales

![lost](https://i.onthe.io/smngoz1rcp8gmbvf2g.1cbea5c7.jpg)

---

### Cart checkout & revenue

![revenue](https://i.onthe.io/smngoz749pjo2jle1.bb897682.jpg)

---

### Visits

![visits](https://i.onthe.io/smngoz457816kf9d.188bc7a7.jpg)

---

### Pages views

![views](https://i.onthe.io/smngoz1olhdh3c1s4g.e45b2036.jpg)

---

### Social activity

![activity](https://i.onthe.io/smngoz7uum43i5qsv.f84405c4.jpg)

---

# [Data As A Service](https://www.librato.com/))

---

# People behind data

---

# [Code for America](http://www.codeforamerica.org/)

---

```
Code for America believes government can work for the people,
by the people in the 21st century.

We build open source technology and organize a network of
people dedicated to making government services simple,
effective, and easy to use.
```

---

# [THE CIVIC TECH ISSUE FINDER](http://www.codeforamerica.org/geeks/civicissues)

---

# Data Driven Assitance

---

# API

> agnostic cookbook

---

# #1
# For a developer...
# be pleasant, please

---

# Pragmatic requirements

---

## use web standards
## friendly explorable via a browser
## simple, intuitive and consistency

---

# [Stripe API Reference](https://stripe.com/docs/api/curl#intro)

---

# API is (just) a developer's UI  

---

# #2
# RESTful URLs and actions

---

REpresentational State Transfer

> Architectural Styles and the Design of Network-based Software Architecture

---

# REST
## Logical resources (things)
## manipulated using HTTP requests methods

---

# GET
# POST
# PUT
# PATCH
# DELETE

---

# NOUNS
### for resources

> students, projects, rents, tweets, cars...

---

# what actions apply to them

---

# CRUD

> Create, read, update and delete

---

* `GET /mentions` - Retrieves a list of mentions
* `GET /mentions/12` - Retrieves the specific mention
* `POST /mentions` - Creates a new mention
* `PUT /mentions/12` - Updates mention #12
* `PATCH /mentions/12` - Partially updates mention #12
* `DELETE /mentions/12` - Deletes mention #12

---

## Just 1 endpoint `mentions`
## No method naming...
## url clean and clear

---

# mention or mentions ?

---

# always use a plural

> consistent and easy life

---

# Relations ?

---

* `GET /mentions/12/topics` - Retrieves a list of topics for mention #12
* `GET /mentions/12/topics/3` - Retrieves the specific topic #3 for mention #12
* `POST /mentions/12/topics` - Creates a new topic for mention #12
* `PUT /mentions/12/topics/3` - Updates topic #3 for mention #12
* `PATCH /mentions/12/topics/3` - Partially updates topic #3 for mention #12
* `DELETE /mentions/12/topics/3` - Deletes topic #3 for mention #12

---

# #3
# Use SSL everywhere, no exceptions

---

# APIs can get accessed from anywhere

> Starbuck, macdo, airports...

---

# simplifies authentication efforts

> access token instead of sign each request

---

# #4
# Have great documentation

---

# API === documentation

---

## Easy to find
## Publically accessible (no sign in...)
## Pastable examples
## Deprecation schedules
## Update communication

---

* [Github](https://developer.github.com/v3/repos/)
* [Twitter](https://dev.twitter.com/rest/public)
* [Mandrill](https://mandrillapp.com/api/docs/users.JSON.html)

---

# #5
# Version via the URL

---

# Always version your API

```
/1.1/followers/ids
```

---

### prevents invalid requests from hitting updated endpoints
### Transition to minor or major version
### Schedule it

---

# #6
# query parameters for advanced filtering, sorting & searching

---

## 1. Keep the base resource URLs as lean as possible
## 2. Complex result could be easily implemented as query parameters

---

# Filtering

```
GET /mentions?type=facebook
```

---

# Sorting

```
GET /mentions?sort=date,rank,sentiment
```

---

# Searching

```
GET /mentions?type=facebook&sort=date,rank,sentiment
```

---

# Aliases for common queries

```
GET /mentions/top_retweets
```

---

# #7

# Limits fields are returned by the API

---

# Use a `fields` query parameter

```
GET /mentions?fields=id,type,author,country,rank,language,sentiment
```

---

# #8

# Return something useful from POST, PATCH & PUT requests

---

# Modification of not provided parameters

---

# #9
# JSON AND ONLY JSON

---

# XML is out the field

---

![xml](http://www.vinaysahni.com/images/201305-xml-vs-json-api.png)

---

# #10

> snake_case vs camelCase ?

---

# JSON so camelCase

> right javascript notation, right ?

---

# Many popular JSON APIs use snake_case

> snake_case is 20% easier to read than camelCase for API

---

# #11

# Free so prevent abuse

---

# standard practice to add some sort of rate limiting

> Take care to notify the consumer of their limits

---

# #12

# Stateless

---

## 1. should not depend on cookies or sessions
## 2. OAuth 2 should be used to provide secure token transfer

---

# #13

# Errors

---

# provide a useful error message in a known consumable format

```
{
  "code" : 504,
  "message" : "Fetching down",
  "description" : "The API server is down, try later"
}
```

---

# #14
# HTTP Code Status

---

* `200 OK`
* `201 Created`
* `204 No Content`
* `400 Bad Request`
* `401 Unauthorized`
* `403 Forbidden`
* `404 Not Found`
* `405 Method Not Allowed`
* `429 Too Many Requests`

---

# An API is a user interface for developers

---

# Put the effort in to ensure it's not just functional but pleasant to use

---

# How ?

---

## PHP
## Python
## Rails
## ASP.NET Web API (C#/.NET)
## Java

---

## Build a RESTful API with
# Node.js

---

## Node
## Express
## Mongoose
## Postman

---

## 1. Handle CRUD item (`students`)
## 2. standard URL
## 3. HTTP RESTful requests
## 4. JSON representation

---

# Structure

```
- api/
    ----- models/
    ---------- student.js
    - node_modules/      
    - package.json      
    - server.js
```

---

# package.json


```
{
    "name": "students-api",
    "main": "server.js",
    "dependencies": {
        "express": "~4.13.3",
        "mongoose": "~4.2.7",
        "body-parser": "~1.14.1"
    }
}
```

---

# Set up the server

```
// server.js
...
var router = express.Router();             

// test route to make sure everything is working
router.get('/', function(req, res) {
    res.json({
      message: 'Welcome to Students API'
    });   
});

// more routes for our API will happen here

// REGISTER OUR ROUTES -------------------------------
// all of our routes will be prefixed with /api
app.use('/api', router);
```

---

![postman](https://cask.scotch.io/2014/04/postman-rest-client-node-api.png)

---

# Database and students model

```
// api/models/students.js

var mongoose = require('mongoose');
var Schema = mongoose.Schema;

var studentSchema   = new Schema({
    'name': 'String',
    'intern': 'String',
    'grade': 'Integer'
});

module.exports = mongoose.model('Student', studentSchema);
```

---

```
// server.js

...

var Student = require('./api/models/student');

...
```

---

# Express Router and Routes

---

route | HTTP verb | Description
----- | --------- | -----------
/api/students | GET | Get all ISN students
api/students | POST	| Create a student
/api/students/:student_id	| GET	| Get a single student
/api/students/:student_id	| PUT	| Update a student with new info
/api/students/:student_id	| DELETE | Delete a student

---

# Creating the Basic Routes

---

## Creating a Bear

```
POST /api/students
```

---

```
router.route('/bears')
  .post(function(req, res) {
    var student = new Student();      
    student.name = req.body.name;  
    student.intern = req.body.intern;  
    student.grade = req.body.grade;  
    student.save(function(err) {
      if (err) {
        res.send(err);
      }
      res.json({ message: 'Student created!' });
    });
  });
```

---

## Getting All students

```
GET /api/students
```

---

```
router.route('/students')
  .get(function(req, res) {
    Student.find(function(err, students) {
      if (err) {
        res.send(err);
      }

      res.json(students);
    });
  });
```

---

## Getting a single student

```
GET /api/bears/:bear_id
```

---

```
router.route('/students/:student_id')
  .get(function(req, res) {
    Student.findById(req.params.student_id, function(err, student) {
        if (err){
          res.send(err);
        }
        res.json(student);
    });
  });
```

---

# ETC, ETC, ETC...

---

# Conclusion

---

# No conclusion
