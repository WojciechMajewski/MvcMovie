# MvcMovie
 Internet Applications Assignment

Answers:
1. What are the responsibilities of each layer of the MVC architecture and how are they
connected?

Model - Responsible for adding, removing and maintaining data, gives the data to the controller
View - Data representation, generates User Interface, using data from the Model through the Controller
Controller - Connects the View and the Model, processes data from the Model and passes to the View

2. What are the naming conventions for models, controllers, controller actions, views folders
and views themselves?
controllers - 'Controller' suffix
controller actions - using built-in convention for controller names that use the form [name]Controller
models - no standard convention
views - named like the action calling them
views folders - named like their controllers

3. How to pass data from controllers to views (2 options)?
Using a dictionary like ViewData or using view model

4. How to map URLs to controller actions?
Using Controller Routing with a pattern

5. How to restrict controller actions to be executed only via certain HTTP request types (e.g.,
only via POST)?
Using an attribute like [HttpPost] or [HttpGet]

6. How to make sure a controller action can only be called through a form on our website and
not through some external request?
By using an anti-forgery token

7. Where do you define data validation and how do you ensure it in views and controllers?
Defined in a Model class, enforced by ModelState.IsValid function ih Controllers and asp-validation functions in Views