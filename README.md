# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

## Checks for Understanding ##

1. Define CRUD.

Stands for basic functions you can perform on data in a database
 - Create -> Add new data
 - Read-> Veiw or retrieve data
 - Update -> Change exsisting data
 - Delete -> Remove data

Matching Verbs
 - GET -> Read
 - POST -> Create
 - PATCH/PUT -> Update
 - DELETE -> delete
   
2. Define MVC.

Model Veiw Controller - it's a way to organize your code so that everything has a clear role and responsibility. I found a metaphor that kinda helped...

Think of it like dividing up jobs in a restaurant ->

 - Model is like the kitchen —> it deals with the data and logic. If your app is a to-do list, the Model would be the part that knows what a "task" is, how to save it in the database, and how to find it later.
 - View is what the customer sees —> like the menu or the plate of food. In a web app or an API, this is what gets sent back to the user (HTML or JSON, for example).
 - Controller is the waiter —> it takes the user’s request (like “add a new task”), talks to the kitchen (Model) to make it happen, and then brings the result (View) back to the user.
   
What two files would you need to create/modify for a Rails application to respond to a GET request to /api/v1/tasks, assuming you have a Task model.
 - You'd need to add a routes.rb file within the config folder -> youll need to edit this to tell it that when someone sends a get request to this route it needs to access the controller and run the action defined 
 - Also a tasks_controller.rb in the api/v1 folder -> this is where youll define the action and how it will function

What are params? Where do they come from?
 - It is a hash like object that holds the data coming in from the client?
   
What is the purpose of a serializer?
 - It conversts JSON before returning it to the client -> this way you can modify what model attributes are being returned - without this it will return all model attributes
