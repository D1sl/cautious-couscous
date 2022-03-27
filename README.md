# cautious-couscous
Week 13 - E-commerce backend

## Assignment
```
GIVEN a functional Express.js API
WHEN I add my database name, MySQL username, and MySQL password to an environment variable file
THEN I am able to connect to a database using Sequelize
WHEN I enter schema and seed commands
THEN a development database is created and is seeded with test data
WHEN I enter the command to invoke the application
THEN my server is started and the Sequelize models are synced to the MySQL database
WHEN I open API GET routes in Insomnia for categories, products, or tags
THEN the data for each of these routes is displayed in a formatted JSON
WHEN I test API POST, PUT, and DELETE routes in Insomnia
THEN I am able to successfully create, update, and delete data in my database

```

### Installation

1. Create a `.env` file in the root directory, and insert the following code, replacing the `DB_USER` and `DB_PW` fields with your MySQL login information
```
DB_NAME='ecommerce_db'
DB_USER=''
DB_PW=''
```
2. Run `NPM I` to install all required dependencies
3. Login to `MySQL Shell` and run `SOURCE db/schema.sql`.
4. Run `NPM RUN SEED` to enter placeholder data into your database. If the seeding fails, make sure that you have a `ecommerce_db` database in MySQL.
5. Run `NPM START` to start the server

### Usage
You can run POST, GET, PUT and DELETE requests, easiest by using `Insomnia`. 

#### Examples:
Run GET requests to:
- /api/products
- /api/categories
- /api/tags

Run POST and PUT requests as below:

`/api/tags`
```
{
	"tag_name": "Violet"
}
```

`/api/products`
```
{
    "product_name": "Scarf",
    "price": 200.00,
    "stock": 3,
    "tagIds": [1, 2, 3, 4]
}
```
`/api/categories`
```
{
	"category_name": "Videos"
}
```


## Video (click to open)
[![Alt text](https://i3.ytimg.com/vi/3iwq8Mw-HME/maxresdefault.jpg)](https://www.youtube.com/watch?v=3iwq8Mw-HME)

## Links
* [Repository](https://github.com/D1sl/cautious-couscous)
* [Video](https://www.youtube.com/watch?v=3iwq8Mw-HME)