# MVC Blog

## Project Description

This project uses the Model-View-Controller (MVC) paradigm to create a blog-style website where developers can create an account, edit their information, make posts, edit posts, and comment on other user's posts.

## Tools Used to Create This Project

* JavaScript ES6
* Node.js
* Express.js
* dotenv (npm package used to store environmental variables used in a project locally so sensitive data like root passwords are not exposed on GitHub)
* MySQL
* Sequelize (npm package for integrating MySQL and Node.js)
* bcrypt (npm package for password hashing)
* handlebars (npm package for a template engine used for html and javascript integration on the front-end)
* Heroku (hosting platform)
  * JawsDB (a Heroku add-on for hosting the MySQL database)

## Usage

The app was deployed to heroku and it says that the build succeeded every time I try to upload it/host it but when visiting the app it does not render so I am unsure why this is happening. 

[HerokuLink](https://mvc-blog-stuff.herokuapp.com/)

How it should be working is that it will render a home page which will include any existing blog posts that were posted. There is also navigation that takes me to the homepage and I am unable to interact with the other pages without being prompted to sign up or sign in. After creating a username and password my credentials get saved to the database.

Once logged in, I can interact with the other navigation links and can post comments on posts that are already being displayed. When I create a new blog post the title and contents of the post are saved and I am redirected back to the dashboard where my post is now being displayed. I have the option to delete and edit my posts and then it will redirect me back to the dashboard where the content has updated. The logout button will log me out but I set a timeout function to automatically time me out after being idle for a while.