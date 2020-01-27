# Mod 3 - Final Project - Hypothesis Testing.
Read Me

#Project Summary:
Given Northwind db, answer stated question and create and answer 3 more hypothesis using the data found in the sql db.
Date used:  Northwind_small.sqlite

files included:  

Readme.md                   - this file
index.ipynb                 - (Jupyter Notebook)
LICENSE.md                  - License
Northwind_small.sqlite      - SQL db with our northwinds data
Northwind_ERD.png           - Schema of our db
Northwind_ERD_unpdated.png  - Schema of our db (latest version)
OrderDetailHighlight.PNG    - Highlight of OrderDetail table

# Questions to Explore
Q1 - "Does discount amount have a statically significant effect on the quantity of a product in an order?  If so, at what level(s) of discount?"
Q2 - "Does discounting impact individual skus?" Our first questions is looking at order quantity as a whole, but in business we want to know how individual products behave.

Q3 - "Does our product catalog demonstrate price elasticity of demand? Highlight skus to further explore" Where we are really getting with this is understanding if we are maximizing revenues or just introducing pricing disparity for the sake of doing so.

Q4 - "Where should we prioritize our sales efforts?" Is our sales team where they should be?

# Process and Design

Summary:   
For the most part, this project was fairly straight forward.   Develop a hypothesis and test it.   As a former consultant it was interesting to dive a bit deeper into raw data as opposed to the clean nice "business-level" data you get post processing.  

As seen in the answering of Question 1, there are many permutations of asking the same question in the name of creating profit because there are just so many different levers one can pull.   When we discussed discounting, we were free to interpret the word "discount" and the word "order" as we saw fit.   In the end I tried to show how the design of the question played a major role in the answer we sought.

Process:

We broke down the few elements of this question and found the data to answer each.

Discount:  We used two separate definitions of discount during our analysis.  Straightforward definition would the % off given by the sales team.  This shows up in the discount column.  A more creative way to define discount would be a product that has a price less than the maximum price we found.

Order:  Much the same can be said for order.  Since an OrderID could be comprised of multiple productIds, which were their own line item, we could define an order as 1 line or 1 orderID with the sum of products involved.

Goal:  break down the data so we would be able to find the statistics needed to calculate probability.   
This included us finding the variance means of our targeted categories, the number of samples, etc.

# Findings:
Discounting seems to influence quantity sold but not improve top level sales figures.
Additionally, some carriers perform better than others.


End of Mod 3 project
