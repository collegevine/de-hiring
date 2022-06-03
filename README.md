# Take Home Problem

## Logistics

First and foremost: Thank you so much for taking the time to work on this project! We really appreciate it. A couple important notes:

1. We've timed the exercise to take about two hours, so please try not to take any longer than that. We're not expecting perfection and are not trying to trick you!
2. Please, please, _please_ reach out if you have any questions about the task, setup, or anything else. We'd be happy to help.
3. We're planning to discuss your solution in your interviews, you please bring it with you and be prepared to discuss!

## Setup

First, please fork this repo so that you can check in any code you write when working on this problem.

Additionally, this take-home problem relies on a couple of tools:

* S3
* A database

Please set up a SQL database on your local machine to use in this exercise. For instance, you might use the official Postgres Docker image, which you can spin up and access as follows:

Pull the image
```bash
docker pull postgres
```

Run Postgres in the background
```bash
docker run \
  --name postgres \
  -p 5455:5432 \
  -e POSTGRES_USER=admin \
  -e POSTGRES_PASSWORD=admin \
  -e POSTGRES_DB=postgres \
  -d \
  postgres
```

You can then use the following URL to connect to your database: `postgres://admin:admin@localhost:5455/postgres`. Feel free to use a non-Postgres SQL flavor or run your database without Docker as well -- whatever is easiest for you.

## Task

* Please ingest the data (supplied in the next section) into your database.
* Do any data cleanup you think is appropriate and model your schema however you like!
* Once you have the data ingested and modeled, please dump your database to a `.sql` file and check it into your fork of the repo.
* Once you have the data in your database, please write a query that determines the number of students that applied to each of the schools with an acceptance rate >= 40%. (**Note: _Each_ meaning "one row per school"**)

## Data

We've supplied some data on students and their admissions results at different universities, which can be found at the following URLs in S3:

* https://cv-de-hiring.s3.amazonaws.com/users.csv
* https://cv-de-hiring.s3.amazonaws.com/school_lists.csv
* https://cv-de-hiring.s3.amazonaws.com/school_list_items.csv
* https://cv-de-hiring.s3.amazonaws.com/schools.json

## What we're looking for

Here are the main criteria we'll use to evaluate your solution:

* Thoughtfully considered data model
* Code clarity
* Code documentation and testing
* Scalability of solution
* Query accuracy


