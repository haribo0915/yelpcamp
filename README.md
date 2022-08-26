# 🏕 YelpCamp

<a href="https://yelpcamp-v3.herokuapp.com/">
 <p align="center">
  <img src="https://res.cloudinary.com/da63zuuon/image/upload/v1661537372/yelpcamp_ujh6hx.png" alt="Campground"
 </p>
</a>

[🔗 yelpcamp-v3.herokuapp.com](https://yelpcamp-v3.herokuapp.com/)

# Features

- Responsive web design (RWD)
- User Authentication and Authorization
- Flash messages responding to user interaction
- RESTful API

```
-------------------------------------------------------------------------
User Routes
-------------------------------------------------------------------------
[Method]  [Route]
GET       /                       Landing page
GET       /login                  Request the user login page
GET       /logout                 Request the user logout page
GET       /register               Request the user edit page

-------------------------------------------------------------------------
Campground Route
-------------------------------------------------------------------------
[Method]  [Route]
GET       /campgrounds            Fetch all campgrounds
GET       /campgrounds/new        Request the campground adding page
GET       /campgrounds/:id        Show the campground information
PUT       /campgrounds/:id        Update campground information (all)
PATCH     /campgrounds/:id        Update campground information (part)
DELETE    /campgrounds/:id        Delete a campground
GET       /campgrounds/:id/edit   Request the campground editing page

-------------------------------------------------------------------------
Review Route
-------------------------------------------------------------------------
[Method]  [Route]
POST      /campgrounds/:id/reviews        Create a new review
DELETE    /campgrounds/:id/reviews/:rid   Delete review
```

# Technologies

- [Bootstrap](https://getbootstrap.com/) - Powerful, extensible, and feature-packed frontend toolkit
- [Node.js](https://nodejs.org) - Node.js® is a JavaScript runtime built on Chrome's V8 JavaScript engine.
- [Express](https://expressjs.com//) - Fast, unopinionated, minimalist web framework for Node.js
- [MongoDB](https://www.mongodb.com/) - NoSQL database for
  modern applications
- [Mongoose](https://mongoosejs.com/) - Elegant MongoDB object modeling for Node.js
- [Passport](https://www.passportjs.org/) - Simple, unobtrusive authentication for Node.js
- [EJS](https://ejs.co/) - Embedded JavaScript templating engine

# Getting Started

Step1. Clone this repository.

```bash
$ git clone https://github.com/haribo0915/yelpcamp.git
```

Step2. Install dependencies via NPM.

```bash
$ cd yelpcamp
$ npm install
```

Step3. Create free acounts on the following services:

- [Cloudinary](https://cloudinary.com/): image storage
- [Mapbox](https://www.mapbox.com/): map api

Step4. Please reference ".env-example" file to create ".env" file under the root directory of the project:

```bash
CLOUDINARY_CLOUD_NAME=<cloudinary_cloud_name>
CLOUDINARY_KEY=<cloudinary_key>
CLOUDINARY_SECRET=<cloudinary_secret>
DB_URL=<url>
SECRET=<salting_secret>
MAPBOX_TOKEN=<mapbox_token>
PORT=<port>
```

Step5. Run the web server and open a browser to visit [http://localhost:8080/](http://localhost:8080/).

```bash
$ npm start
```
