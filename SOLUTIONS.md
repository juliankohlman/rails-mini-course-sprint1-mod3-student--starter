## Rails MVC

### 1. What controller and action handles the data from the form submission?

- The `tasks_controller` along with both the `#create` and `#show` actions.

---

### 2. What controller and action would be used if you did a `GET` request on the `/users route`?

- The `users_controller` along with the `#index` action.

---

##### 3. Write out the step-by-step process that your rails application will take to render the `tasks/new route`.

- Steps
  - `GET` request sent from browser to `Rails Router`
  - `Rails Router` passes route `tasks/new` along to `TasksController` for processing
  - The `#new` action captures the `@task` variable and passes it to the `new` view
  - The view uses `.erb` to render a page in html
  - The `TasksController` passes the `html` back to the browser.

---

##### 4. What file is responsible for managing the mapping between your application and the `tasks` database table?

- `routes.db` inside of `config` dir, at the projects root.

---

## Rails RESTful Actions

##### 5. Explain all 7 of the RESTful actions in Rails

- List each action by its name
- Explain which HTTP verbs pair with each action
- Write a short sentence for each action that summarizes what it does

1. `#index` - `GET` - display a list of all of `resource type`
2. `#new` - `GET` - return a form for creating a new `resource type`
3. `#create` - `POST` - create a new `resource type`
4. `#show` - `GET` - display a specific `resource type`
5. `#edit` - `GET` - return an html form for editing `resource type`
6. `#update` - `PATCH/PUT` - update a specific `resource type`
7. `#destroy` - `DELETE` - delete a specific `resource type`

---

## Use Rails Console to Create a User

- Commands
  - `rails console`
  - `User.connection`
  - `user_one = User.create`
  - `User.first`
  - `user_two = User.create`
  - `User.last`
