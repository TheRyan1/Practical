# ToDo Tracker

## About : 
In this task you will create a fullstack ToDo application using the following technologies

- NodeJS
- ExpressJS
- ReactJS

#### You are not required to incorporate a database solution. 
#### All data will persist for the duration of the express server uptime.
#### There are 4 ToDos already hardcoded for you in an array named FakeDB. 
#### Use this array when adding / removing ToDos.


## Installation Instructions : 
1. Create a fork by logging into github and then clicking fork on the top right corner of the https://github.com/TheRyan1/Practical page.

2. Clone a copy of the project template 
```
git clone 'your forked repository link'
```
3. Install react base dependencies
 ```
npm run client-install
 ```
4. Install server base dependencies
 ```
npm install
 ```
### Folder Structure:
```
root - /practical
 |-- index.js
 |-- node_modules (for server)
 |-- package.json (for server)
 |-- client root /practical/client
     |-- src
     |-- public
     |-- node_modules
```
           
### Express Server Dependency List > Make sure you are in the server root
```
npm install express
npm install cors
```
### React Dependency List > Make sure you are in the client root
```
npm install react-router-dom
npm install axios
```
You can use react-query if you don't want to go through the hassle of cancelling promises. 
```
npm install react-query
```
### Tips : 
- React-Router-Dom example : https://react-hhnm7g.stackblitz.io/home
- Axios example
```JavaScript
//Get Request
const getData = async()=>{
 let response = await axios.get('api_URL');
 let data = response.data
 return data
}

//Post Request
const SubmitData = async()=>{
 let user = 
 {
  username:"Steve",
  password: "12345"
 }
 
 let response = await axios.post('api_URL',user);
 let data = response.data
 return data
}
```

## Server Checklist : 

* Install express
* Create a new express application
* Implement CORS middleware
* Create routes
  * Get All ToDo list items (GET)
  * Delete ToDo list item (DELETE)
  * Create ToDo list item (POST)
  * Update ToDo list item (GET with route parameter)

## React Front end Checklist : 

* Create components (Components)
  * HomePage.jsx (View All ToDos)
  * CreatePage.jsx (Create ToDo)
  * EditPage.jsx (Edit ToDo)
  * DeletePage.jsx (Delete ToDo) 
  * NavBar.jsx
  * Footer.jsx
* Create routing with react-router-dom
* Interact with backend API using Axios
* Implement styling of your choice. CSS / MUI / Bootstrap

### React Tips:

1) Make use of the useLocation Hook to pass data when navigating to the delete and update pages
2) Make use of the useState hook to manage the state of each component
3) Make use of useEffect hook to load all ToDo items when navigating to the HomePage


## Bonus Points :
* Implement a database
* Implement JWToken for authentiction
* Implement A Register feature
* Implement a Login feature
* Only display ToDos for the currently logged in user

