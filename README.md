## This repository was created to showcase how to setup MongoDB database on your local machine and run NodeJS application with it

<a href="https://www.mongodb.com/" target="_blank" rel="noreferrer"> <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/93/MongoDB_Logo.svg/2560px-MongoDB_Logo.svg.png" alt="mongodb" width="512" height="138"/></a>

### MongoDB Local Setup on macOS (assuming that you already have node and brew installed)

- open terminal
- brew tap mongodb/brew
- brew install mongodb-community@6.0
- brew services start mongodb-community

### Import database from collections folder

- clone this repo
- npm install mongodb@4.10
- from the terminal navigate to the db-collections folder
- run `mongoimport --db=cooker --jsonArray users.json`
- run `mongoimport --db=cooker --jsonArray recipes.json`

### Run NodeJS programms

- from the VSCode terminal
- run `node basic-test.js`
- run `node find-one.js`
- run `node find.js`
- run `node find-sorted-limited.js`
- run `node recipe-search.js`
