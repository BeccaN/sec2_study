# sec2_study
A review of the different topics covered in section 2 of the SE online PT Flatiron program. 

SQL - language for managing databases
    * We dont write a lot of this anymore, thanks to ActiveRecord!
        
ORMs - Object Relational Mapping, it is both a design pattern concept (Object Relational Mapping) and noun (Object Relational Mapper)
    * This is something we can create ourselves, but Active Record replaces this
    * In the past we had to build a whole class where we wrote out all our CRUD methods

ActiveRecord - a Ruby gem that creates the Model methods in the MVC system
    * Active Record covers the CRUD methods needed to interact with the db
    * Can we create customized ActiveRecord methods? Is this suggested? (Avi Building a SiteGenerator video, having the custom 'songs' method that included an error message)
    * can overwrite methods and add additional functions

Rack - A Ruby gem, middleware (between web server and framework)

HTML - hypertext markup language, it builds the structure of a webpage

CSS - cascading style sheets, it adds style to the webpage (makes it look pretty)

Sinatra - A Ruby gem, Ruby based web framework
    * Built on top of Rack
    * Light weight web framework - smaller, minimal, less code/stuff (requires the developer to potentially have to code more)
    * web frameworks are great because they add lots of great methods that let us handle HTTP requests and responses (simplifies a lot of stuff...)

MVC - Model, View, Controller 
    * This is a design pattern commonly used for developing user interfaces
    * Model - the object/instance version of our db (it does all the CRUD stuff to the db)
    * Controller - central command center, bridges between Model and View
    * View - what the user sees/interacts with

CRUD - Create, Read, Update, Destroy
    * covered with ActiveRecord

REST - standards on how to build a app, making it easier for systems to communicate with each other. 
    * Statelessness - information required for that route is entirely covered from there, and doesn't get passed along to other routes. 
    * RESTful route - uniform naming system

Shotgun - Ruby gem that uses HTTP to create a server to locally run our web app

Tux - Ruby gem that lets you access your db in the terminal and perform CRUD operations from ActiveRecord
    * debugging
    * Useful when you want to test how the model is sending/saving info on the db

Bcrypt - Ruby gem, it lets us handle passwords more safely
    * it cyptifies a user password in the database to help secure it against hackers
    * so if my password is '1234' then bcrypt changes it to an equivalent crazy looking thing to be stored on the db (like hp57h34pq5734op578h)

Sessions - stores the user login info into a hash (session[:user_id]), lets us use that hash in other routes
    * used to store any information that we want to persist amongst the different routes
    * defined in ApplicationController

Helper methods - Helper class creates logic/methods that we can use in our views, to help eliminate the amount of Ruby code (logic) we have to put in the views (ERB, embedded ruby) 
    * defined in Application Controller, and then the other controllers inherit them from ApplicationController

ERB - embedded ruby, .erb files are how we make our views using ruby and html. 

Migrations - ruby file, that let us to make changes to the structure of our db

RSPEC - DSL(domain specific language) for writing tests
