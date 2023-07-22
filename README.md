# InstaBackend Project 

## Frameworks and Language Used

<p align="center">
<a href="Java url">
    <img alt="Java" src="https://img.shields.io/badge/Java->=8-darkblue.svg" />
</a>
  <a href="Spring Boot url" >
    <img alt="Spring Boot" src="https://img.shields.io/badge/Spring Boot-3.0.6-brightgreen.svg" />
</a>
<a href="Maven url" >
    <img alt="Maven" src="https://img.shields.io/badge/maven-3.0.5-brightgreen.svg" />
</a>
  
<a >
    <img alt="MySQL" src="https://img.shields.io/badge/MySQL-blue.svg">
</a>
</p>

The InstaBackend project is developed using the Spring Framework, with Spring Boot as the primary framework for building the backend. The main language used for development is Java.

## Data Flow

### 1. UserController
The `UserController` class handles incoming HTTP requests related to user operations on Instagram and directs them to the appropriate service methods.

- `signUpInstaUser()`: This endpoint responds to a POST request to "/user/signup" and signs up a new Instagram user based on the provided user data in the request body.

- `sigInInstaUser()`: This endpoint responds to a POST request to "/user/signIn" and handles user sign-in using the provided credentials.

- `sigOutInstaUser()`: This endpoint responds to a DELETE request to "/user/signOut" and signs out an Instagram user based on the provided email and token in the request.

- `createInstaPost()`: This endpoint responds to a POST request to "/post" and creates a new post on Instagram based on the provided post data and user email in the request.

- `removeInstaPost()`: This endpoint responds to a DELETE request to "/post" and removes an Instagram post based on the provided post ID and user email in the request.

- `addComment()`: This endpoint responds to a POST request to "/comment" and adds a comment to an Instagram post based on the provided comment data and commenter email in the request.

- `removeInstaComment()`: This endpoint responds to a DELETE request to "/comment" and removes an Instagram comment based on the provided comment ID and user email in the request.

- `addLike()`: This endpoint responds to a POST request to "/like" and adds a like to an Instagram post based on the provided like data and liker email in the request.

- `getLikeCountByPost()`: This endpoint responds to a GET request to "/like/count/post/{postId}" and returns the like count for a specific Instagram post based on the provided post ID and user email in the request.

- `removeInstaLike()`: This endpoint responds to a DELETE request to "/like" and removes an Instagram like based on the provided like ID and liker email in the request.

- `followUser()`: This endpoint responds to a POST request to "/follow" and allows a user to follow another user on Instagram based on the provided follow data and follower email in the request.

- `unFollowUser()`: This endpoint responds to a DELETE request to "/unfollow/target/{followId}" and allows a user to unfollow another user on Instagram based on the provided follow ID and follower email in the request.

### 2. Model Classes
The project defines various model classes to represent entities such as `Admin`, `AuthenticationToken`, `Comment`, `Follow`, `Like`, `Post`, and `User`. These classes are mapped to corresponding database tables using JPA annotations.

### 3. Repository
 The Repository layer typically be implemented using Spring Data JPA. It manages the interactions with the underlying database and provides methods for CRUD operations on the entities.


## Data Structure Used in Your Project

The primary data structures used in the InstaBackend project are various model classes, such as `User`, `Post`, `Comment`, `Like`, `Follow`, `Admin`, and `AuthenticationToken`. These classes represent different entities and their relationships, which are managed and persisted in the database.

## Project Summary

The InstaBackend project is a backend application built using the Spring Framework with Java as the primary programming language. It provides various endpoints to handle user-related operations on Instagram, such as signing up, signing in, signing out, creating posts, adding comments, adding likes, following/unfollowing users, etc. The project follows a structured data flow pattern, with controllers handling incoming requests, services implementing business logic, and a repository for data access to interact with the underlying database.

## Author

👤 **Mohammad Ashif**

* GitHub: [Mohammad Ashif]( https://github.com/ashifdeveloper)

    
---

## 🤝 Contributing

Contributions, issues and feature requests are welcome.
    
---
    
## Show your support

Give a ⭐️ if this project helped you!
    
---
    
## 📝 License

Copyright © 2023 [Mohammad Ashif]( https://github.com/ashifdeveloper).<br />
    
---
