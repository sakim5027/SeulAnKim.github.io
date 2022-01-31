---
layout: post
title: PetGuru Project Retrospective
subtitle: CodeStates Final Project Retrospective
gh-repo: codestates/PetGuru-server
gh-badge: [star, fork, follow]
cover-img: /assets/img/PetGuru/PetGuru_Logo.png
tags: [Node.js, Express, MySQL, Sequelize, AWS(EC2, RDS), Multer, JWT, PM2]
comments: true
---
<br>

## Looking Back the PetGuru project

  ![MainPage](../assets/img/PetGuru/Website/07. Main Page.png)

This was the second group project I experienced in the CodeStates bootcamp. In this project, I worked with 3 other teammates, and participated as the Back-end web developer. During the 6 weeks, our team worked as a group and went through all the process from the service planning to the website building. Below are the things I felt while going through this first group project.

<br>

## Contribution

<br>

- Position: Back-end
- Stack: Node.js, Express.js, MySQL, AWS EC2, AWS RDS, SequleizeORM, JWT, pm2, multer, multer-S3


**[ Team Collaboration (SR) ]**

- Came up with Service ideas
- Selected the Development Concepts for the Service
- Created Flow chart and Wire Frame using Miro & Figma

**[ DATABASE ]**

1. DB Diagram Schema Design
    - Designed Database Schema using DB Diagram

<br>
    
2. MySQL Database Build up
    - Built MySQL Database using Sequelize ORM
    - Created Database Model Association
    - Created & Maintained RDS DB instance
    

**[ API ]**

1. Server API endpoint Design
    - Designed API endpoint
    - Created API Document using Gitbook
    - Built routers in Express framework of NodeJS

<br>
    
2. Response Build up for each API endpoints
    - Pet(pet information) CRUD
    - Missing(missing pet post) CUD
    - Missing_answer(issing pet post reply) CRUD
    

**[ Image Upload ]**

1. MULTER & MULTER-S3
    - Saved the image data from Client to AWS S3 using MULTER-S3
    - Provided Client the S3 image link


**[ AWS Deployment ]**

1. Deployment & Server Management using AWS
    - AWS EC2
    - AWS RDS
    - pm2



<br>

### Server endpoint API Design

In this project, I had an opportunity to design whole API endpoints & responses for the each endpoints. It was a challenge for me, especially since I had to come up with all the possible endpoints that would be needed in the website BEFORE building the website. So, I had to use my imagination and rely on the Wireframes and Flowcharts we created in the planning stage. 

In order to do this, me and another Back-end developer (we had 2 Back-end developers including me in this project) first came up with basic endpoints we thought we might need and left notes on the points that might need update. Then, we discussed about those points and edited them as we proceeded. Below is how we worked on this API endpoint design in Notion:

  ![API1](../assets/img/PetGuru/API endpoint 1.png)
  ![API2](../assets/img/PetGuru/API endpoint 2.png)

Once we finished listing possible endpoints, I created API Document using Gitbook. In this process, I could learn about **HTTP Status Code** used in API responses. Below are some of the frequently used HTTP status codes:

**[1×× Informational]**

- 100 Continue
- 101 Switching Protocols
- 102 Processing

**[2×× Success]**

- 200 OK
- 201 Created
- 202 Accepted
- 204 No Content

**[3×× Redirection]**

- 300 Multiple Choices
- 301 Moved Permanently
- 302 Found
- 303 See Other
- 304 Not Modified
- 305 Use Proxy
- 307 Temporary Redirect
- 308 Permanent Redirect

**[4×× Client Error]**

- 400 Bad Request
- 401 Unauthorized
- 403 Forbidden
- 404 Not Found
- 409 Conflict

**[5×× Server Error]**

- 500 Internal Server Error
- 503 Service Unavailable
- 504 Gateway Timeout
- 505 HTTP Version Not Supported
- 511 Network Authentication Required
- 599 Network Connect Timeout Error


After this, I created API endpointes and built responses for each endpoints using routers in Express framework. Then we tested the request & responses using Postman. This stage went rather smoothly, especially since I already planned & designed all API endpoints and responses in the API Document. I felt the importance of planning & creating appropriate API Documents in the planning stage.

* [API Document (Gitbook)](https://petguru.gitbook.io/petguru-gitbook/ "https://petguru.gitbook.io/petguru-gitbook/")

<br>

### MySQL Database Build up

In this project, I built relational database using MySQL. At first, I created Model & did migration using Sequelize in the terminal. After that I created Modeal association and connected each Database Models since this was relational database. For example, User table and Pet table has 1:N relationship, and this could be created with below code:


```javascript
db.User.hasMany(db.Pet,{
  foreignKey: 'user_id',
  sourceKey: 'id'
});

db.Pet.belongsTo(db.User,{
  foreignKey: 'user_id',
  targetKey: 'id'
});
```

Also, I made the sequelize to sync if Database is modified by adding below code:

```javascript
db.sequelize.sync({
	alter : true
})
```

In order to check whether the data went into the database successfully, I used MySQL Workbench. With this app I could see the table visually, and it helped me a lot especially in testing process.

  ![MySQLWorkbench](../assets/img/PetGuru/MySQL Workbench.png)


<br>

### Multer & Multer-S3 Image uploader


<br>

### Project Deployment


<br>

### Learning from the Teammates



<br>

### Resizing the Project

