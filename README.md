# deleg.io
*deleg.io* is a project management application primarily meant for medium to large sized projects. 

# Features
- Agile principles, SCRUM methodology (user stories, epics, tasks etc.)
- Project task hierarchy
- Chat with project members
- Streamlined task completion process

# Technology Stack
## Backend
- [NodeJS 14.9.0](https://nodejs.org/en/)

### Backend libraries and frameworks
- [Mongoose](https://mongoosejs.com/)
- [Express](https://expressjs.com/) and [Nest](https://nestjs.com/)
- [Nodemon](https://nodemon.io/)

#### Template engine
- [ejs](https://ejs.co/) (Embedded JavaScript)
    - No need to learn a new syntax, just embed native JS

## Frontend
- [Angular](https://angular.io/)
- Native JS, ECMAScript

### Frontend libraries and frameworks
- [LeaderLine](https://anseki.github.io/leader-line/)
- [PlainDraggable](https://anseki.github.io/plain-draggable/)
- [Panzoom](https://anvaka.github.io/panzoom/)

## Database
- [Mongo](https://www.mongodb.com/)


# Guides

## General
- Keep the backend separate from the frond end (make two seperate Git repositories)
- Coding best practises
    - ECMAScript coding convention
        - camelCasing, etc.
    - Modularity
    - Readability
        - A single functions performs a single task
        - The name of a function should be very descriptive and explicit
    - Comments to explain large or less obvious code snippets

## Development of Angular and Nest
Both the Angular app and the Nest app can be run seperately. The Angular app can simply refer

## Combining Angular and Nest for production
1. In the Angular project directory, run
    - ```ng build```
2. Copy the files from the Angular project's ```dist``` directory to the Nest project
    - Paste all but ```index.html``` into the Nest project's ```public``` directory.
    - Paste ```index.html``` to the Nest project's ```views``` directory
        - Change the file type to match the template engine 
            - ```index.html``` to ```index.ejs```
3. In the Nest application, run
    - ```nest build```
    - ```nest start```
