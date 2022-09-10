# Places app

Simple mern project about places.

## Functionalities of this server

Users apis:<br>
api to get all users<br>
api to sign up a user<br>
&emsp;> returns back a token in the responose
api to login a user<br>
&emsp;> returns back a token in the responose

Places apis:<br>
api to get places by user id<br>
api to get a place by id<br>
api to create a place<br>
&emsp;> protected, expects a token in the request header<br>
api to edit a place<br>
&emsp;> protected, expects a token in the request header<br>
api to delete a place<br>
&emsp;> protected, expects a token in the request header<br>

## Running the project locally.

1. download and unzip project.<br>
   open the project in a code editor e.g. Visual Studio Code.<br>
   Requires npm and node.js on your development setup.<br>

2. rename nodemon copy.json to nodemon.json<br>
   (using this file for development)<br>

3. Requires google maps api<br>
   (both frontend and backend can use the same key)<br>
   Sign up at: `https://developers.google.com/maps`<br>
   create a new account, then enable the geocoding api and maps javascript api.<br>
   Go to the Credentals tab and copy that api key<br>
   Replace the value of REACT_APP_GOOGLE_API_KEY in:<br>
   &emsp;.env<br>
   &emsp;.env.production<br>

4. Requires mongodb<br>
   Sign up at: `https://www.mongodb.com/`<br>
   Create a new cluster.<br>
   For the next few steps, mern, db_user and password<br>
   can be interchangeable for other values.<br>
   Just make sure the corresponding values are used in nodemon.json.<br>
   Create a new database named mern<br>
   Under mern database, create these collections:<br>
      &emsp;places<br>
      &emsp;users<br><br>

   Go to the database access tab.<br>
   Add a new database user with:<br>
      &emsp;username: db_user
      &emsp;password: password
      &emsp;user should at least have access to the mern database<br><br>
      
   Go to the network access tab.<br>
   Add an ip addreess: 0.0.0.0/0<br>
      &emsp;but if you want, you can always restrict to certain ip addresses

5. In the terminal, type in:
   &emsp;npm install (install dependecies)<br>
   &emsp;npm run start (run the project locally)<br>

