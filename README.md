# Code Notes

**Currently in Developement**

> * Maintained by: `Adam Botma`, `Jingwen Wu`, `John Nguyen`, `Maison Keiser`

* Used React.js to create all HTML elements (virtual DOM) to dynamically display data received from the PostgreSQL database via API server created using Node.js

* Used Express to retrieve user's notebook data

* Used Amazon Web Services EC2 for web, API server, and PostgreSQL database

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

  1. Update a note

  ### The client can send DELETE requests to the server to remove from the database to:

  1. Delete a note

### Devices
* The app can be properly viewed on a desktop and on an iPad in landscape mode.

## Lessons Learned
  1. Accessing the local storage using React.js functions and dynamically display data using React.js virtual DOM functions
  2. Creating a basic yet responsive user interface using React.js and Bootstrap 4
  3. Leveraging Object Oriented Programming to organize code into components
  4. Creating an API server using Node.js to process requests from and send data to the client
  5. Storing and handling session data using Express session
  6. Experienced the full development process of deploying the web and API server into AWS EC2 and creating a PostgreSQL database

## Live Site
* The live version of the app can be viewed [here](https://code-notes.johnnguyencodes.com).

### Demos

* Desktop

<img src="https://user-images.githubusercontent.com/61361957/96650366-a3377c80-12e7-11eb-937e-c8c7a744b2ea.gif" width="600" alt="Desktop Demo Gif"/>

* iPad - Landscape

<img src="https://user-images.githubusercontent.com/61361957/96650371-a5014000-12e7-11eb-9b19-635b6baec0f2.gif" width="600" alt="iPad - Landscape - Demo Gif"/>
