# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
One purpose of a backend is to allow users on the same web app to interact with each other.
Without a backend, users would not be able to do this, limiting what our application is capable of. Another
purpose is to securely store data that can persist over time.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
Model
```

Which layer in the MVC pattern communicates with the model?

```md
Controller
```

Why don't we use views in our interpretation of the MVC pattern?

```md
Because we build our own Client 'views' with HTML/Handlebars/Javascript etcetera.
```

What does C.R.U.D stand for?

```md
CREATE, READ, UPDATE, DESTORY.
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
Controller.
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
Index (READ), Create (CREATE), Show (READ), Update (UPDATE), Destroy (DESTROY).
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
- The server receives the GET requests and uses routes to find out which controller to use.
- The web server then uses the dispatcher to create a new controller, call the action and pass the parameters.
- Controllers parse user requests and tell the model to perform the request.
- The model talks to the database, stores and validates data, and performs the business logic.
- The model returns a response to the controller.
- The controller returns the response body and metadata to the server.
- The server combines the raw data into an HTTP response and sends it to the user.
```

What is the command to generate a new rails-api app?

```bash
rails-api new app_name -T --database=postgresql
rails-api new <api_name> [-OPTIONS]
```

What is the command to start an instance of a rails server?

```bash
bundle exec rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
bundle exec rake db: drop
bundle exec rake db: create
bundle exec rake db: migrate
bundle exec rake db: seed
bundle exec rake db: examples
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
rails-api g scaffold pet name:string age:integer
```
