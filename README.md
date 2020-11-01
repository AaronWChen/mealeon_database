# What is this repo?

This repo contains code to supplement MeaLeon. MeaLeon works as is, but does not have enough recipes in its database. To simplify MVP and allow for easier project silo-ing, I decided to created a separate repo that just contains work to improve the database.

# Sources

1. The original MeaLeon web scrape from Epicurious

2. Updated Epicurious web scrape

3. Allrecipes (https://www.allrecipes.com/recipes/86/world-cuisine/)


## Table of Sites

| Site                                                             | Why?                           | Labeled? | Number of Recipes | Usage?                                  |
|------------------------------------------------------------------|--------------------------------|----------|-------------------|-----------------------------------------|
| Nytimes.com                                                      | Good recipes                   |          |                   |                                         |
| Epicurious.com                                                   | Good compilation, labeled      | Yes      |                   | Model Training, Model Testing, Database |
| Bonappetit.com                                                   | Good recipes                   |          |                   |                                         |
| Seriouseats.com                                                  | Good recipes                   | Yes      |                   | Database                                |
| Kadiafricanrecipes.com                                           | African source                 |          |                   |                                         |
| Allrecipes.com                                                   | Lots of recipes, labeled       | Yes      |                   | Database                                |
| Yummly                                                           | Lots of recipes                | No       |                   | Model Training, Model Testing           |
| Food.com                                                         | Lots of recipes, crowd sourced | No       |                   | Model Training, Model Testing           |
| Africanbites.com                                                 | African source                 | Yes      |                   | Database                                |
| Congocookbook.com                                                | African source                 | Yes      |                   | Database                                |
| https://www.allnigerianrecipes.com/                              | African source                 | Yes      |                   | Database                                |
| https://www.myburntorange.com/recipe/                            | African source                 |          |                   |                                         |
| https://www.sanjanafeasts.co.uk/blog/browse-recipes-by-category/ | African source                 |          |                   |                                         |
| http://www.executivemamaput.com/recipes/                         | African source                 |          |                   |                                         |
| https://9jafoodie.com/recipe-index-2/                            | African source                 |          |                   |                                         |
| https://www.theafricangourmet.com/search/label/African%20food    | African source                 |          |                   |                                         |
|                                                                  |                                |          |                   |                                         |
|                                                                  |                                |          |                   |                                         |
|                                                                  |                                |          |                   |                                         |

# Future Steps

1. Create new requirements.txt
    Likely need just scraping for one part
    Containerize the scraper?
        Containerization should make it easier to run on other hardware


2. Find sites and scrape

3. Incorporate into database
    Two databases:
        1. Used for training and testing classifier. Cannot display the original recipe, but still has a label that can help (see Yummly)

        2. Used for displaying results to user. Must have accessible weblink

4. Train classifier to augment database with new recipes
