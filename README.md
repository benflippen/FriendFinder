# Friend Finder
---

**[Deployed Heroku link](https://regular-friend.herokuapp.com/)**

Do you enjoy taking personality tests and Regular Show?  After filling out a quick survey, my friend-matching algorithm will pair you with a character from Regular show that is the most compatible to you.

## Technologies Used
---
- Node.js
- JavaScript
- Express.js
- HTML
- Bootstrap

## Functionality
---
1. The `server.js` file sets up the Express server, specifying the npm packages, port number, and also the routes.

2. There are 2 separate HTML files (`home.html` and `survey.html`) that serve as the front-end portion of our code; they determine what the user sees (the homepage and the survey, which will also show the resulting best match)

3. (`htmlRoutes.js` and `apiRoutes.js`) determine the back-end logic (based on the request being made, the response that gets sent to the browser); the HTML routes display the survey and the homepage based on the URL that is accessed, and the API routes send back existing content in our server-side data

4. Best match is calculated by finding the friend with the minimal difference in scores and then sending that friend to the browser as a JSON object.
