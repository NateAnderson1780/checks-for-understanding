## Week Three Recap

### Instructions
Fork this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

1. What are the 3 main features in an ERD?
Entities, attributes, relationships
2. Create an ERD for the following database: Restaurants, Customers, Items, Ingredients, Beverages, Orders, Vendors.
done
3. What is the entry at the command line to create a new rails app?
rails new (appname) -d (database)
4. What do Models generally inherit from in rails?
ActiveRecord::Base
5. What do Controllers generally inherit from in a rails project?
ApplicationController
6. How would I create a route if I wanted to see a specific horse in my routes fitle assuming I'm sticking to standard conventions and that I didn't want other CRUD functionality?
resources :horses, only: [:show]
7. What rake task is useful when looking at routes, and what information does it give you?
rake routes. Gives you prefix, verb, uri pattern, and controller#action.
8. What is an example of a route helper? When would you use them?
playlists_path. takes you to a specific page in your site.
9. What's the difference between what `_url` and `_path` return when combined with a routes prefix?
path just returns the domain, while url includes the entire url.
10. What are strong params and why are the necessary?
params that you have to make a decision on to allow for mass update.
11. What role does `form_for` play in helping us create our forms?
It uses the object passed in to determin what it is a form for.
12. How does `form_for` know where to submit the user's input?
names for label and text fields.
13. Create a form using a `form_for` helper to create a new `Horse`.
<%= form_for(@horse) do |f| %>
  <%= render partial: "shared/errors", locals: {target: @horse} %>
  
  <%= f.label :name %>
  <%= f.text_field :name %>
  
  <%= f.label :breed %>
  <%= f.text_field :breed %>
  
  <%= f.submit %>
<% end %>
14. Why do we want to validate our models?
For a number of different reasons. To make sure the attributes that are included for the model are being used is one possibility. Another validation property is uniqueness which ensures the same value will not be entered twice. 
