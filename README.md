# Code Notes

**Currently in Development**

Code Notes is a dynamic CRUD web application built for web development students to organize their notes, documentation resources, flash cards, and code examples in one central app.

> * Maintained by: `John Nguyen`, `Adam Botma`, `Jingwen Wu`, `Maison Keiser`

### Technology Overview

* Used React.js to create all HTML elements (virtual DOM) to dynamically display data received from the PostgreSQL database via API server created using Node.js
* Used Express to retrieve user's notebook data
* Used Amazon Web Services EC2 for web, API server, and PostgreSQL database


### Technologies Used

* React.js
* Node.js
* Express
* PostgreSQL
* Webpack 4
* Bootstrap 4
* HTML5
* CSS3

## Feature Overview
### The client can send GET requests to the server, and in return can receive and display the data in HTML format to:
  1. View all available notebooks
  2. View all available notes of a particular notebook
  3. View a note, along with difficulty, added resources and code examples, if any
  4. Search for a note by providing a note title
  5. Search for a note by providing a note tag
  6. Search for a note by difficulty
  7. View all available flashcard decks
  8. View/study all available flashcards of a particular deck
  5. Search flashcards by providing a tag

### The client can send POST requests to the server to add to the database, and in return can receive and display the data in HTML format to:

  1. Create a new notebook
  2. Create a new note for a particular notebook
  3. Add difficulty, tags, resources, and code examples to a note
  4. Create a new flashcard for a note

  ### The client can send PUT requests to the server to update the database, and in return can receive and display the data in HTML format to:
  
  1. Update a note, along with its difficulty, added resources and code examples, if available

### The client can send DELETE requests to the server to remove from the database to:

  1. Delete a note

### Devices
* The app can be properly viewed on the desktop and on an iPad in landscape mode.

## Lessons Learned
  1. Accessing the local storage using React.js functions and dynamically display data using React.js virtual DOM functions
  2. Creating a basic yet responsive user interface using React.js and Bootstrap 4
  3. Leveraging Object Oriented Programming to organize code into components
  4. Creating an API server using Node.js to process requests from and send data to the client
  5. Storing and handling session data using Express session
  6. Experienced the full development process in a team environment by:
     * prototyping the visual design through Figma
     * designing a database schema on DB Designer and creating it with PostgreSQL
     * overall project management on MeisterTask
     * collaborating on a single codebase through pull requests, code review and resolving code conflicts on GitHub
     * deploying the web and API server into AWS EC2.

## System Requirements
* Ubuntu Linux 18.04 LTS
* Node.js 10
* PostgreSQL 10
* pgweb
* NPM 6

## Set Up Environment
1. Clone the repo

```
git clone https://github.com/johnnguyencodes/code-notes.git

cd class-notes
```
2. Install all dependencies with NPM
```
npm install
```

3. Import the example database to PostgreSQL

```
npm run db:import
```

4. Create a .env file in the root directory and paste in the following:

```
PORT=3001
DEV_SERVER_PORT=3000
DATABASE_URL=postgres://dev:lfz@localhost/classNotes
SESSION_SECRET=secret
SESSION_EXPIRY=28800000
```

4. Start the PostgreSQL service
```
sudo service postgresql start
```

5. Start the server
```
pgweb --db=classNotes
```

6. Start the project.  Once started, you can view the application by opening http://localhost:3000 in your browser.
```
npm run dev
```



## Live Site
* The live version of the app can be viewed [here](https://code-notes.johnnguyencodes.com).

### Preview

* Desktop

<img src="https://user-images.githubusercontent.com/61361957/98852563-b2a07600-240c-11eb-86db-9f7855a2576d.gif" width="600" alt="Desktop Demo Gif"/>
