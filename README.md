# API DOCUMENTATION

This is a simple stateless microservice in Nodejs, with three major features -
- Posts management
- Comments management

## Usage
To start the backend project; follow these steps:

Run `cd server`

Run `npm i`  or `yarn` to install all the dependencies

Run `sails lift` to start the project

The backend is accessible via `http://localhost:1337` by default

Additionally, you can run `npm test` to run the tests included in the project.

**NOTE:** Your server has to be running for the `integration tests` to complete. Also, it is recommended to have an internet connection because the database is hosted online.

## Routes
This are the available endpoints at the backend:
### Create Post
- `POST http://localhost:1337/post` 

    Example Request body:
    ```javascript
        {
            title: 'title',
            description: 'description',
            author: 'author'
        }
    ```
    
### Get Post By Id

- `GET http://localhost:1337/post/:id`

    Example Request body:
    ```javascript
        {  
        }
    ```

### Search Post
- `POST http://localhost:1337/posts` 

    Example Request body:
    ```javascript
        {
            size: 10,
            page: 1
        }
    ```

### Create Comment
- `POST http://localhost:1337/comment` 

    Example Request body:
    ```javascript
        {
            postId: 10,
            message: 1
        }
    ```
        
  
### Search Comment
- `POST http://localhost:1337/comments` 

    Example Request body:
    ```javascript
        {
            page: 1,
            size: 10
        }
    ```
        
# FRONTEND DOCUMENTATION

## Usage
To run this project follow these steps:

Run `cd client`

Run `npm i`  or `yarn` to install all the dependencies

Then run `npm start` to start the project

The frontend is accessible via `http://localhost:3000` by default
