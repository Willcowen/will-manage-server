***WILL MANAGE***

**Project Description**

I've created a project management tool, which allows users to register, login and keep track of their own workflow, via an up to date list of tasks. A user can add new tasks, edit or delete existing tasks.

**Screenshots of the application.**

Screenshots can be found on the client repository here: https://github.com/Willcowen/will-manage-client

**Setup instructions**

To run this project locally on your machine, you'll need to do the following:

1. Clone this repository.

2. Use npm install to install the projects dependencies from the package.json file.

3. Go to the client repo here, and repeat steps 1 & 2: 

 https://github.com/Willcowen/will-manage-client

4. You will need a database set up for this, this project is using PostgreSQL. Instructions on how to set this up can be found here:

 https://www.learmoreseekmore.com/2020/09/postgresql-elephantsql-cloudserv.html

5. Go to the .env.example file on the server and update [YOUR-URL] with both main and shadow database URL's. If unsure, please refer to above link. Rename the .env.example file to .env

6. Then type npm start on both client and server directories to run the application.

**Approach to implementation**

The front end on this application was setup using react, react-router-dom, react-beautiful-dnd (drag and drop) and MUI. The back end was setup using express, postgres and prisma.

**Learnings**

The biggest challenge for me was learning a new library, IE react-beautiful-dnd. Whilst this was a pain to get up and running, it makes the app function in the way I wanted it to.

If I was to create something similar again, I would probably focus more on functionality, before styling the app in the later stages of its development. Set up an Endpoint on the back end, ensure it works with Thunder Client, or Postman/Insomnia then integrate the front end for this end point. This would allow for continuous integration between the front and the back end. Even if the app didn't quite look how I wanted it to at that moment. 

Another challenge was figuring out the logic within rendering items correctly when a task or item is dragged and dropped.