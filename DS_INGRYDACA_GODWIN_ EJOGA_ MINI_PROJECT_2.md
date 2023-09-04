#### Q1: You are workig for an online marketplace. Users often search for a  products using keywords. Given a list of product names and their corresponding IDs, design a function that allows users to input a keyword and quickly find the product they are looking or, implement a linear algorith to search for the keyword in the list of product names and return the corresponding product ID.


```python
# Defining a class to represent product

class Product:
    def __init__(self, product_id, name):
        self.product_id = product_id
        self.name = name

        
products = [
    Product(1, "Samsung"),
    Product(2, "Nokia"),
    Product(3, "Motorola"),
    Product(4, "Iphone"),
]

def search_product(keyword, product_list):
    results = []
    for product in product_list:
        if keyword.lower() in product.name.lower():
            results.append(product)
    
    return results

search_keyword = input("Enter a keyword to search for a product: ")

# Perform Product Search

found_products = search_product(search_keyword, products)

# Dsiplay Results.

if found_products:
    print("Product Found:")
    for product in found_products:
        print(f"Product ID: {product.product_id}, Name: {product.name}")
              
else:
    print("No matching product found")
        
#Welcome/Closing Meassge

print("Thanks you for reaching out")
```

    Enter a keyword to search for a product: samsung
    Product Found:
    Product ID: 1, Name: Samsung
    Thanks you for reaching out
    


```python

```


```python

```


```python

```


```python

```


```python

```
