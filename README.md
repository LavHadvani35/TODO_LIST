**********************Todo List Application Using MERN****************************

Todo List web application using MERN stack is a project that basically implements basic CRUD operation using MERN stack (MongoDB, Express JS, Node JS, React JS). 

The users can read, add, update, and delete their to-do list in the table using the web interface. 
The application gives a feature to the user to add a deadline to their task so that it user can be reminded of the last day to complete the project.


**********************Approach to Create Todo List:**************************

In Frontend, the react component called “Todo” is used to display tasks, deadlines and its status and form to add new todo item with edit and deletion feature.

In Backend, application fetches data from MongoDB using backend API called “/getTodoList”. 
New data can be added to the database using “/addTodoList” API. 
“/updateTodoList/:id” API is used to edit the existing specific data from the table. 
“/deleteTodoList/:id” API is used to delete the specific data from the table.


********************Functionalities Of Todo Application:*********************

Add New Todo List: User can add new todo task using the form. On clicking “submit” button, The new data will be saved to database.
Display Todo List: User can view the todo list in table format.
Edit Existing Data: User can click on “Edit” button to make the table row to editable fields. On clicking “Edit” button, new buttons call “Save” will be created. “Save” button is to update the edited data to database.
Delete Existing Data: User can click on “Delete” button available in the table row to delete the data from database.


****************************Frontend Code:*****************************

App.js: This is our main file which routes to the Todo component.
Todo.js: This component contains all the logic for displaying Tasks, Status of tasks and deadlines of the tasks fetched from database in table format, adding new todo list to database, deleting existing todo from database and editing existing todo in database.


****************************Backend Code:******************************
Server.js: This is a file which contains logic to start the backend server, APIs to interact with database.
todoList.js: This is a model file called a wrapper of the Mongoose schema. This file is used to define the schema of table that stores the todo list.