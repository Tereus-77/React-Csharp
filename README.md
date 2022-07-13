# Getting started

### Clone

Clone this repository

```
git clone https://github.com/Tereus-77/React-Csharp
```

Then, change to repository folder

```
cd React-Csharp
```

### Run

Requires

-   [SQL SERVER](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)
-   [.NET Core 3.1 SDK](https://dotnet.microsoft.com/download)
-   [NodeJS](https://nodejs.org/en/)

**Run the Web Api**

First, restore dependencies

```bash
$ dotnet restore
```

To run the tests

```
$ dotnet test
```

Create database tables with the sql script located in ./database/scripts/TodoList.sql

Then, run the project with with

```bash
$ dotnet run --project src/TodoList.WebApi
```

**Run the React app**

Fill the env file located in ./src/todo-list-spa with the api url:

```
REACT_APP_API_URL=http://localhost:5000
```

```bash
# Install dependencies
$ npm install --prefix src/todo-list-spa

# Starting the project
$ npm start --prefix src/todo-list-spa
```
