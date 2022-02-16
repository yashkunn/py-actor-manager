# Cinema hall manager

- Read [the guideline](https://github.com/mate-academy/py-task-guideline/blob/main/README.md) before start

In this task, you should create a manager for the dataclass `CinemaHall`.

#### 1. Create dataclass inside `models.py` module
`CinemaHall` should have the following attributes:
- id - unique identifier for each cinema hall
- capacity - max number of visitors
- description - general information about hall

#### 2. Create database
Create a database `cinema` where will be stored entries with data about different cinema halls.
Create a table `cinema_hall` with corresponding columns.
Now, you are ready to create a manager.

#### 3. Create manager inside `managers.py` module
Create `CinemaHallManager` class that should provide **CRUD** operations. 
It should create a connection to the database inside the constructor.
The manager should have the following methods:
- `create` - a method that creates a new entry in the `cinema_hall` table
with given properties.
- `all` - a method that returns a list of `CinemaHall` instances from db
- `update` - a method that updates properties for entry with given `id`
- `delete` - a method that deletes entry with given `id` from db

#### 4. Test
Test different methods in the `main.py` module.
