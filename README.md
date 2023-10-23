## To Do List

#### A web application that allows users to create a list of categories of household chores, and add lists of chores to each category.

#### By Brian Scherner

## Technologies Used

* C#
* .NET
* ASP.NET MVC
* MySQL

## Description

This application presents users with a home page where they can add different types of categories of household chores to a list. They can then select a category, and add chores belonging to that category to another list saved for that specific category. Users can also view the details of each chore that they have created. They can add multiple items to a single category as well.

## Setup Instructions

### Install Tools

Install the tools that are introduced in [this series of lessons on LearnHowToProgram.com](https://old.learnhowtoprogram.com/fidgetech-3-c-and-net/3-0-lessons-1-5-getting-started-with-c/3-0-0-01-welcome-to-c).

### Set up Project Database

Follow the instructions in the LearnHowToProgram.com lesson ["Creating a Test Database: Exporting and Importing Databases with MySQL Workbench"](https://old.learnhowtoprogram.com/fidgetech-3-c-and-net/3-3-database-basics/3-3-0-08-creating-a-test-database-exporting-and-importing-databases-with-mysql-workbench) to create a `to_do_list_with_ef_core` database with an `items` and `categories` table.

### Set up and Run Project

1. Select the green button that says `Code`, and clone this repository.
2. Open your terminal and navigate to this project's production directory called `ToDoList`.
3. In the production directory `ToDoList`, create a new file called `appsettings.json`.
4. In `appsettings.json`, put in the following code, replacing the `uid` and `pwd` values with your own username and password for MySQL. For the LearnHowToProgram.com lessons, always assume the `uid` is `root` and the `pwd` is `epicodus`. Example below:

{

    "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=music_organizer_with_mysqlconnector;uid=root;pwd=epicodus;",
      "TestConnection": "Server=localhost;Port=3306;database=music_organizer_with_mysqlconnector_test;uid=root;pwd=epicodus;"
    }

}

5. In the production directory `ToDoList`, run the command `dotnet watch run` to launch the project in development mode with a watcher.
6. Open the browser to [https://localhost:5001](https://localhost:5001). If you cannot access localhost:5001 it is likely because you have not configured a .NET developer security certificate for HTTPS. To learn about this, review this LearnHowToProgram lesson: [Redirecting to HTTPS and Issuing a Security Certificate](https://old.learnhowtoprogram.com/fidgetech-3-c-and-net/3-2-basic-web-applications/3-2-0-17-redirecting-to-https-and-issuing-a-security-certificate).

## Known Bugs

Application is functioning fully as intended. I would like to add some CSS styling later on, though.

## License

MIT

Copyright(c) 2023 Brian Scherner