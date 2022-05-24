# Take Home Problem

## Setup

This take-home problem relies on a couple of services:
* S3
* (Heroku) Postgres

For S3, data is in a public bucket called `cv-de-hiring`. 

## Data

We've supplied some data on students and their admissions results at different universities, which can be found at the following URLs in S3:
* https://cv-de-hiring.s3.amazonaws.com/users.csv
* https://cv-de-hiring.s3.amazonaws.com/school_lists.csv
* https://cv-de-hiring.s3.amazonaws.com/school_list_items.csv
* https://cv-de-hiring.s3.amazonaws.com/schools.json

## Task

Please ingest the data into the database we've provided. Model it however you like and think makes sense with any tools you want! Once you have the data in the database, write a query that determines the number of students that applied to each of the schools with an acceptance rate >= 40%.

