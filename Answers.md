# DB-Assignment

1. Explain the relationship between the "Product" and "Product_Category" entities from the above diagram.
   
Ans:  The relationship between “Product” and “Product_Category” entities:
      The “Product” entity is related to the “Product_Category” entity through the “category_id” attribute in the “Product” table. Specifically, each product in the “Product” table has a foreign key “category_id” that references the primary key “id” of the “Product_Category” table. This establishes a many-to-one relation between the "Product" and "Product_Category" entities, where multiple products can belong to a single category.


   
2. How could you ensure that each product in the "Product" table has a valid category assigned to it?

Ans:  To ensure that each product in the “Product” table has a valid category assigned:
      Firstly, It is essential that we make sure the “category_id” field in the “Product” table is not nullable, meaning that every product must have a category ID. Following this, we need to set up foreign key constraints on the “category_id” column in the "Product" table, so that it references the primary key, which is "id" column in the “Product_Category” table. This ensures that every category ID in the “Product” table matches an existing ID in the “Product_Category” table.
