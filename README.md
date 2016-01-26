In the previous lesson we looked at a brief and fairly dry lesson on the MVC (Model-View-Controller) framework. Here again is the original version: 

*There are three parts to MVC; model, view, controller. The model manages the fundamental behaviours and data of the application. This could be retrieved from a database or any other sort of data store.*

*The view is the user interface. This takes data from the model and displays it nicely for the user. Any user interaction in the view is then handed over to the controller.*

*The controller receives user input and makes calls to the model and view to update/modify either. This keeps the main aspects of our application separate.*

## Here's how we reworked it: 

*We could create create a web application in one file, with thousands of lines of code in the same document. It would work. But it would also present us with some very big challenges. It would be close to impossible to debug our program, and our code would be virtually unreadable.
Instead, we use frameworks (Sinatra being one of them), to separate an application's code by function and make writing, reading, and debugging code a much more pleasant and simple experience.*

*The Model-View-Controller paradigm is a popular way of building frameworks for web applications - it provides a separation of concerns where groups of files have specific jobs and interact with each other in very defined ways. In a nutshell:*

*Models: The 'logic' of a web application. This is where data is manipulated and/or saved.*
*Views: The 'front-end', user-facing part of a web application - this is the only part of the app that the user interacts with directly. Views generally consist of HTML, CSS, and Javascript.*
*Controllers: The go-between for models and views. The controller relays data from the browser to the application, and from the application to the browser.*

*The Restaurant Analogy*
*If you've ever been to a restaurant, you'll know that there is a clear separation of concerns that takes place. The person cooking the food is not the same as the person delivering the food, and the person eating the food is someone completely different. Let's think of MVC as if it were a restaurant.*

*Models*
*First, there are the cooks (the models) that make the food. They take orders (from the waiter), and prepare the customer's meal. Once ready, they give it to the waiter to deliver to the customer.
In Sinatra, models are generally written as Ruby classes. Models can also connect to databases to persist data. Think of models as the main logic behind your web application.*

*Views*
*The customers (views) place orders and receive food. The orders are placed with the waiter, who takes them back to the kitchen.
In Sinatra, views are written as .erb files, consisting of HTML and embedded Ruby (Ruby code written within html). They are what the user actually sees when they use your web application.*

*Controllers*
*The waiters (controllers) shuttle between the kitchen and the front of the restaurant. They take requests from the customer to the kitchen, and take prepared meals from the kitchen to the customer. Without the waiter, our customers would be hungry and our chefs would have nothing to do.
In Sinatra, controllers are written in Ruby and consist of 'routes' that take requests sent from the browser ("GET this data", "POST that data"), run code based on those requests by using models, and then render the erb (view) files for the user to see.*



<a href='https://learn.co/lessons/example-improving-our-not-so-great-body' data-visibility='hidden'>View this lesson on Learn.co</a>
