# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
// It is to make a web app functional and interactive
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
// The model
```

Which layer in the MVC pattern communicates with the model?

```md
// The database and the controller
```

Why don't we use views in our interpretation of the MVC pattern?

```md
// Because we are not using rails but js to interact with the HTML and generate the views.

```

What does C.R.U.D stand for?

```md
// Create, read, update, delete
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
// The controller
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
// Index, create, show, update, destroy
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
// your response here
```

What is the command to generate a new rails-api app?

```bash
// rails new my_api --api
```

What is the command to start an instance of a rails server?

```bash
// rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
// rails console,
 ActiveRecord::Migration.drop_table(:name table)
 rails generate
 rake db migrate,
 rails seeder
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
// rails generate model Pet name:text age:integer
```
