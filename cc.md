Ruby on Rails uses MVC development pattern to create apps.  

M, which stands for model, represents database tables. An example of a model maybe User, Post, Comment. Models are always written has singular words. A rake db:migrate must be done when a new model is generated. Models also allow for an interface for CRUD actions to take place on data models. (Create, Read, Update and Destroy)

V, which stands for views, represents what the user actually sees on the brower. There is a viewes folder in all rails apps, which is where all the html.erb files are contained. If you have a user model, a users folder must be created in the views folder that contains all relevant html.erb files inside it.

C, which stands for controller, is a bridge that binds together the models and views. The code written inside the controller files indicates what happens when a request is initiated. All queries should be established in the controller. 

A rails request is made when a user enters a URL in the browser, making a request to an application. After a request is made, the rails router matches the URL to a controller and a controller action. The router searaches for that controller and performs all the code in the controller file. If the def index method action in the controller file is empty, the router knows to display whatever is in the views index file that corresponds with the same name as the controller. Lastly, whatever is in the views files displays what the user will be in the browser

Each aspect of the MVC model needs to coexist and function with one another in order for the application to work properly. In order for everything to work cohesively together, proper routes need to be created and established with the use of HTTP request types. All the routes are created in the routes.rb file. 
