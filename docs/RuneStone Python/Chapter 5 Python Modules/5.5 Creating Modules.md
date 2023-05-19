# 5.5 Creating Modules

- Every time you’ve written a Python script you’ve created a module
- A Python module is just a Python source code file.

```python
"""
coffee_shop.py
The coffee shop module contains functions and contains variables
important to implementing a coffee shop.
"""

# Set some variables
shop_name = "Runestone Brew House"
coffee_sizes = ["small", "medium", "large"]
coffee_roasts = ["hot chocolate", "light", "medium", "dark", "espresso"]
```

- This is a Python script named `coffee_shop.py`that contains three variables: `shop_name`,`coffee_sizes`, and `coffee_roasts`. The `shop_name`is a string, `coffee_sizes`is a list containing strings, and `coffee_roasts`is also a list containing strings.
- How can we use the `coffee_shop`module? We can import it and use it in other Python source code files.

```python
#coffee_customer.py
import coffee_shop

# Output the information we know from the module
print("Welcome to", coffee_shop.shop_name)
print("Available sizes:", coffee_shop.coffee_sizes)
print("Available roasts:", coffee_shop.coffee_roasts)
```

- **The module files must be in the same directory on your computer for Python to know how to import them automatically**
- We use **dot notation** to grab the `shop_name`, `coffee_sizes`, and `coffee_roasts`variables from the `coffee_shop`module
- Variables aren’t the only thing we can place in modules though… We can put any valid Python code in them.

### Let’s improve our coffee shop

```python
"""
coffee_shop.py
The coffee shop module contains functions and contains variables
important to implementing a coffee shop.
"""

# Set some variables
shop_name = "Runestone Brew House"
coffee_sizes = ["small", "medium", "large"]
coffee_roasts = ["hot chocolate", "light", "medium", "dark", "espresso"]

def order_coffee(size, roast):
    """
    Take an order from a user
    :param size: a string containing one of the coffee_sizes
    :param roast: a string containing one of the coffee_roasts
    :return: a message about the coffee order
    """
    return "Here's your {} coffee roasted {}".format(size, roast)
```

- The old file contents are present, but now there’s also an `order_coffee`function that takes two arguments, `size`and `roast`

We’ve got a function in our module now, let’s use it.

```python
#this is coffee_customer.py
# Import the module with coffee_shop functionality
import coffee_shop

# Output the information we know from the module
print("Welcome to", coffee_shop.shop_name)
print("Available sizes:", coffee_shop.coffee_sizes)
print("Available roasts:", coffee_shop.coffee_roasts)

# Get some inputs from the user
order_size = input("What size coffee do you want? ")
order_roast = input("What roast do you want? ")

# Send the order to the coffee shop module
shop_says = coffee_shop.order_coffee(order_size, order_roast)
# Print out whatever it gave back to us
print(shop_says)
```

### Further Expansion of Example

```python
"""
coffee_shop.py
The coffee shop module contains functions and contains variables
important to implementing a coffee shop.
"""

# Set some variables
shop_name = "Runestone Brew House"
coffee_sizes = ["small", "medium", "large"]
coffee_roasts = ["hot chocolate", "light", "medium", "dark", "espresso"]

def order_coffee(size, roast):
    """
    Take an order from a user
    :param size: a string containing one of the coffee_sizes
    :param roast: a string containing one of the coffee_roasts
    :return: a message about the coffee order
    """
    return "Here's your {} coffee roasted {}".format(size, roast)

def add_milk_please(fat_content):
    """
    Pretend like we're adding some milk to a coffee
    :param fat_content: a string or integer containing the milkfat content
    :return: a message about having added the milk
    """
    return "I've added the {}% milk".format(fat_content)

def give_tip(tip_amount):
    """
    Take a tip from the user, then be happy about it
    :param tip_amount: the tip amount
    :return: nothing
    """
    print("Thank you so much!  We don't make a ton of money.")

    # Not having a "return" statement causes our function to return None
```

```python
#coffee_customer.py
# Import the module with coffee_shop functionality
import coffee_shop

# Output the information we know from the module
print("Welcome to", coffee_shop.shop_name)
print("Available sizes:", coffee_shop.coffee_sizes)
print("Available roasts:", coffee_shop.coffee_roasts)

# Get some inputs from the user
order_size = input("What size coffee do you want? ")
order_roast = input("What roast do you want? ")

# Send the order to the coffee shop module
shop_says = coffee_shop.order_coffee(order_size, order_roast)
# Print out whatever it gave back to us
print(shop_says)

# See if the user wants to add milk
add_milk_response = input("Do you want to add milk (y/n)? ")
# Convert the response to lowercase, then check for a "yes" answer
if "y" in add_milk_response.lower():
    milk_fat = input("What percent milk do you want added? ")
    shop_says = coffee_shop.add_milk_please(milk_fat)
    # Print out whatever it gave back to us
    print(shop_says)

# They better give a tip...
print("THAT'S GOOD COFFEE!  Very good.  Your brain is working again.")
print("You better give a tip.")
tip_amount = input("Tip amount? ")
coffee_shop.give_tip(tip_amount)
```

### Module Comments

- It is important to include header comments in your module that explain what the module does.

### Function Comments

- Functions are the next chapter, but the comments used here demonstrate a common Python documentation style.