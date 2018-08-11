# Datacamp

## **Chapter-1 : Selecting columns**

## select all comumn
* `SELECT * FROM tabe;` - সব কয়টা কলাম সিলেক্ট করার জন্য 
## select single column
* `SELECT column_name FROM table;` - ঐ টেবিল থেকে শুধুমাত্র ঐ কলাম টা সিলেক্ট করার জন্য
## select multiple column
* `SELECT column1,column2 FROM table;` - Multiple column সিলেক্ট করার জন্য 

## select distinct
Often your results will include many duplicate values. If you want to select all the unique values from a column, you can use the DISTINCT keyword.

`SELECT DISTINCT language FROM films;`

## Comments
`--` This is a comment


## count

`SELECT COUNT(*) FROM people` - এক বা একাধিক কলামে  কয়টা লাইন আছে সেটা count করে দেখায় 

`SELECT COUNT(column_name) FROM people` - ঐ column এ কয়টা not null ভেলু আছে ঐটা দেখাবে 

It's also common to combine COUNT with DISTINCT to count the number of distinct values in a column.

`SELECT COUNT(DISTINCT column_name) FROM table_name`

## **Chapter-2 : Filtering rows**


### Filtering result : 

`WHERE` clause always comes after the FROM statement
### Simple filtering of numeric values :
Get all details for all films released in 2016.

`SELECT * FROM films WHERE release_year = 2016;`

