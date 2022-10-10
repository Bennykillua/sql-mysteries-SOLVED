# SQL Murder Mystery: Can you find out whodunnit?

This project will solve and document the responses to SQL Murder Mystery
Can you find out whodunnit?

To learn more about it check out [mystery.knightlab.com](https://mystery.knightlab.com/)

# Steps taken

This command in this file is specific to SQLite. You can try it out on the IDE in this [website](https://mystery.knightlab.com/)

## what do we know? 

A crime has taken place and the detective needs your help. The detective gave you the crime scene report, but you somehow lost it. You vaguely remember that the crime was a ​murder​ that occurred sometime on ​Jan.15, 2018​ and that it took place in ​SQL City​.

## 1. Exploring the Database Structure

We would start by exploring the Run this query to find the names of the tables in this database.

```
SELECT name 
  FROM sqlite_master
 where type = 'table'
```

![fork repository](https://github.com/Bennykillua/sql-mysteries-SOLVED/blob/master/Solved%20solution/images/Table%20overview.png)

## 2. Exploring the `crime_scene_report` table
This will give us details about the police report to find out what other informations the police knows.

Run this query.

```
Select * from crime_scene_report
where date = 20180115
and type = "murder" and city = "SQL City"

```

