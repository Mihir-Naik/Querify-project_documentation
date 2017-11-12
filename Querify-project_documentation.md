# Project Documentation
-- 

- Link for deployed version: [Querify](https://querify.herokuapp.com/)
	
	**Test email: `byran@ga.com` Password: `password`**
- Link for Code: [Github](https://github.com/Mihir-Naik/Querify)

--- 
### Technical Requirements for the project:

* **Build a full-stack application** by making your own backend and your own front-end
* **Design a restful API **
* **Have an interactive front-end**, preferably using a modern front-end framework
* **Be a complete product**, which most likely means multiple relationships and CRUD functionality for at least a couple models
* **Use a database**
* **Implement thoughtful user stories** that are significant enough to help you know which features to build and which to scrap
* **Have a visually impressive design** to kick your portfolio up a notch and have something to wow future clients & employers
* **Be deployed online** so it's publicly accessible
* A **git repository hosted on Github**, with a link to your hosted project

### Project Idea and description:

- The idea for this project came from the web applications like Stackoverlfow, Quora and other similar apps that are so useful in today's world to answer pretty much all the querries. Hence, the name of the project `Querify` that can possibly bring the community together to help each other solve their issues and share their knowledge. 

Querify is a web application designed by collaborating an idea of Questions & Answers app and a platform for Blog posts. User can sign up with their basic details like name, credentials, where they live and their email and password. Logged in users can edit their user profile, delete account or even edit/delete the content posted by them. Once users are logged in, they can select one of the options from their profile page like:

- Post a new question,
- Answer other people's question and cast a vote on other answers,
- Write a new blog post,
- Read others' blog post,
- Comment on others' blog post and also like or dislike the post.

There are some conditional rendering features based on whether logged in user is the owner of the content or not. For example, owner of the content will have varied features like only allowed to view the vote counts on their content or likes for thier content but are allowed to vote and like others' content. Also, only owner of the content can edit/delete the content while others can only view the content.

---

### Technologies used for the project:

- **Git & GitHub for Version Control**
- **Heroku for Deployment**
- **GLIFFY** For [Models / Enitity Relationship Diagram](https://i.imgur.com/VYL6okE.png)
- **[TRELLO BOARD](https://trello.com/b/0XVSVIts/querify-project-4)** For USER Stories. 

#### || 	MERN STACK  ||
 
	- Mongo DataBase
	- Express
	- Node.js
	- React 

#### Dependencies:
	# CLIENT (Front-End)
	
	- React-dom
	- React-router-dom
	- jwt-decode
	- Axios
	- Moment
	- BootStrap 4.0
	
	# SERVER (Back-End)
	
	- bcrypt-nodejs
	- body-parser
	- dotenv
	- jsonwebtoken
	- morgan


### Installation instructions for Developers
- Fork the project from GitHub: [https://github.com/Mihir-Naik/Querify] (https://github.com/Mihir-Naik/Querify)
- From your terminal, go to your workspace and run `git clone (forked repo's link goes here)`
- From within the cloned directory, run `npm install`, which will install all the dependecies for server side application.
- Further down in the directory you will find a directory called `client`, `cd` into the client directory and again run `npm install` which will install all the client side dependecies.
- For Development mode: Client server is set on `PORT: 3000` and Backend/API server is set on `PORT: 3001`.
- Make sure to add your `secret key` for jsonwebtoken in your `.env` file.
- Run `mongod` & `nodemon` from your project root directory.
- Run `npm start` from `client` directory.


- Share your views/opinion via email @ `mdnaik17@gmail.com` with `QUERIFY` in the subject.

--- 

### Challenges/Difficulties Faced during the project

- **Overall understanding of the REACT concepts and how it works.**

Given 4 days of time to develop a full Stack application using MERN Stack after barely 2 weeks of learning REACT was definately a challenge. 
The approach to face the challenge was to do research on how things exactly work in functional programming and try `throw away` codes to understand the concepts. Also, ***`console.log()` was definately the best teacher/helper to understand the processflow and understand functions.***

- **Finding Bugs and Debugging them**

There were few events during testing the application, when a bug was found and it would take some time and effort to find and fix the issue which was actually the best part of the challenge.

For example, While testing the user edit profile feature, it was found that user details were succefully getting updated and saved on the backend but while redirecting to the profile page it was not rendering the most updated information. To resolve this bug, I went through the complete process of going through the code to find any logical errors that might be causing such bug. As expected, it was found that the initial state of the profile page was rendering based on the information of the user that was available at the time of successful log in. When user was redirected to edit profile page, user carried over the information and then updated that information in terms or user's name or credential or anything else. After submitting the request to save the changes, user was redirected back to profile page which would render the old information as the authentication token was not updated either while saving the changes at backend or sending back the updated user and re-rendering it. So to fix the issue, once the user was updated at backend, I had to destory the token attached to that user and create a new token with updated user information and attach it to the user. That updated the state of logged in user and upon rendering the profile page it reflected the succesful changes. 

- **Make the project visually impressive**

The challenge to work on design part of the application was mainly due to the time contstraint and wish to add as many functionalities as possible. To meet the bare minimum requirements of making the project visually designed, bootstrap 4 was used. 

### Future Features / Unsolved Issues

- For now, likes and votes are not limited to only once by any particular user. i.e. A user can like or dilike or vote for any content multiple times.
In future, it would be limited for each user to do any of these things only once. 
- Definately, more designing and imporvement in the user interface is planned for future.


-- 
### ***Documentation By: MIHIR NAIK***

