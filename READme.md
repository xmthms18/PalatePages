# PalatePages

## Technologies
- React
- Node
- Express
- MondoDB
- Oauth
- Possibly TheMealDB APi

## User Stories
- I want to be able to search for different recipes
- I want to be able to add and delete recipes on to my personal "cookbook"
- I want to be able to signup and login with an account
- I want to be able to view recipe details and instructions


## Wireframes
<img src ="D9BBB4C5-6A8F-4A5F-A9C4-04A40DCD7C60.jpeg">

## ERDs

+------------+ one to many +------------+ one to many +-------------+
|   User     | <---------->|  Cookbook  | <------->   | Recipe      |
+------------+             +------------+             +-------------+
| userID     |             | cookbookID |             | recipeID    |
| email      |             | userID     |             | title       |
| password   |             | recipeID   |             | ingredients |
| created_at |             | notes      |             | catogory    |
| updated_at |             | rating     |             | created_at  |
+------------+             | created_at |             | insructions |
                           | updated_at |             +-------------+
                           +------------+


## Restful routes
|---------------------------------------------------------------|
| User Authentication                                           |
|---------------------------------------------------------------|
| POST | /api/users/signup         |                            |
| POST | /api/users/login          | User Login                 |
| POST | /api/users/logout         | User Logout                |
| POST | /api/users/reset-password | Reset User Password        |
|---------------------------------------------------------------|
| Recipe Search and Discovery      |                            |
|---------------------------------------------------------------|
| GET  | /api/recipes/search       | Search Recipes             |
| GET  | /api/recipes/:id          | Get Recipe by ID           |
|---------------------------------------------------------------|
| Users CookBook                                                |
|---------------------------------------------------------------|
| GET    | /api/cookbook           | Get User's Cookbook        |
| POST   | /api/cookbook           | Add Recipe to Cookbook     |
| PUT    | /api/cookbook/:recipeId | Update Recipe in Cookbook  |
| DELETE | /api/cookbook/:recipeId | Delete Recipe from Cookbook|
|---------------------------------------------------------------|

## MVP
- Search/Home page
- Cookbook/User home page
- add delete and create sections in cookbook

## Stretch Goals
- Create custom recipes
- Filtered search ( Breakfast, dinner, italian, etc...)
- Nutrition facts
- Categorized cookbook



# PalatePages
