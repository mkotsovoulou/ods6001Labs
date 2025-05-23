# Programming Problem 8: Web Services and Pandas

> The purpose of this assignment is to test your understanding and application of the concepts discussed up to **week 7**:
>
> - Call a web service
> - Retrieve a JSON Object
> - Load JSON into a Dictionary
> - Parse Data
> - Use Pandas Data Frames

## Specifications
A company has created a webservice to expose its products, their prices and the number of items they have in stock. The API documentation of the webservice, can be found at: https://dummyjson.com/docs/products

Create a program to download the json products and categories data sets from the following web services:
- https://dummyjson.com/products
- https://dummyjson.com/products/categories

Use the data retrieved to:

1. Find the most expensive product in each category and the product name.

2. The total number of items the company has in stock for the specific category.

3. Produce a formatted output, like the following, in a text file called 'stats.txt':
```
CATEGORY           MOST EXPENSIVE PRODUCT           PRICE   CAT STOCK
----------------   -------------------------------  -----   ---------
smartphones        Samsung Universe 9                1249         319
laptops            MacBook Pro                       1749         386
fragrances         Non-Alcoholic Concentrated P       120         397
skincare           Freckle Treatment Cream- 15g        70         470
groceries          Gulab Powder 50 Gram                70         465
home-decoration    Handcraft Chinese style             60         263
```
Display only those categories where a product exists!

4. Display the price of the most expensive product of all in the terminal.

5. Create a pandas data frame from the summary dictionary and produce basic statistics using the describe statement.

6. Extra Challenge: import matplotlib.pyplot and create a bar chart of the product category max prices.


<details>
<summary>
Hint 1 : Nested Loops
</summary>

```
Loop through the categories and in this Loop, iterate over the products.

    - If the product category is equal to the current category from the outer loop

        - add the stock to a categoryStock dictionary.

        - check the product price to see if it larger to the previous "larger" price.

            - if yes, assign this product's price to a largest variable...and the name to another variable

    - Add the final values to another dictionary called summary with key the category and as a value a list of the required information (product name, price and total category stock)
```

</details>

To start the assignment type in the terminal:
```
code assignment8.py
```

## Execute and Test your program

*Remember*: in order to execute your code you type in the terminal:

```
python assignment8.py
```


## Check Your Code

```
check50 mkotsovoulou/ods6001a/main/assignments/assignment8
```


## Submit your code

When you are happy with your solution, download the code and the stats.txt and upload it to Blackboard.

![Image of download](download.png)

# Done!
:tada:
