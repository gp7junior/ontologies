# Ontologies' Repository by G. Pedro Silva Jr

This repository stores my ontologies.

## Ontology N. 1 : My-food-ontology: 

This ontology models information about restaurants, their menus and served dishes.

The intention of this ontology is to feed a Natural Language processing system helping people to find interesting places to eat.

### Hierarchy of classes and their data properties:

* Restaurant - name:string
* Menu - startDate:dateTime, endDate:dateTime 
* Food - price:float, descritption:string
  * Dish - firstCourse,secondCourse,vegetarian:boolean
* Ingredient - allergen:boolean.
* Cuisine
* Location - addres:string, longitude:float, latitude:float

### Object Properties

* Restaurant is specialized in Cuisine,
   * serves Food
   * has Menus
   * is located in Location
* Menu lists Food
* Food is served in Restaurants
* Dish contains Ingredients
* Dish belongs to Cuisine
* Cuisine has dishes
