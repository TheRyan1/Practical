# Web Programming 1 Assessment

## About : 
In this assignment you will create a fullstack ToDo application using the following technologies

- NodeJS
- ExpressJS
- ReactJS

#### You are not required to incorporate a database solution. 
#### All data will persist for the duration of the express server uptime.
#### There are 4 ToDos already hardcoded for you in an array named FakeDB. 
#### Use this array when adding / removing ToDos.


## Instructions : 
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
 

