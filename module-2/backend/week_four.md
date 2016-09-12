## Week Four Recap

### Instructions
Fork this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

* What is a cookie?
it is information for future use that is stored by the server on the client side of a client/server communication.
* What’s the difference between a session and a cookie?
session is stored server side while cookie is stored client side on browser.
* What’s a flash and when do you want to use flashes?
The flash provides a way to pass temporary primitive-types (String, Array, Hash) between actions. Anything you place in the flash will be exposed to the very next action and then cleared out. 
* Why do people say “HTTP is stateless”?
Each request is separate and must contain enough information to hold it's own.
* What’s authentication? Explain.
establishing and confirming a site user's identity.
* What’s the difference between authentication and authorization?
Authen-establishes who you are....author-establishes where you can go
* What’s a before filter?
before filter can be used to set methods with information that is being reused in other methods.
* How do we keep track of a user once they’ve logged in?
sessions
* When do you want to namespace a resource? When do you want to nest a resource? What's the differences between those two approaches?
namespace a resource you dont have a model for the namespace. nest resources when you are attaching objects to each other. 
* At a high level, what tools can you use to implement authorization? How would you use them?
bcrypt, implements secure passwords
* What's an enum, and what advantages does it offer? What data type needs to be in your database to use an enum? Where do you declare an enum?
enum can declare different authentications when you log in. array? In the model (User)
* What are some strategies you can use to keep your views DRY?
partials and helpers
