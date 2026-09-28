# Supermarket Project

This is my first semester python project. It is a supermarket program where you can shop, return things and checkout, and everything is done with a menu.

I made it using only basic python, so there are no functions and no modules in it.

## What it does

- Shows a menu again and again until you choose Quit
- You can shop from 4 categories (Electronics, Fruits and Vegetables, Groceries, Self Care)
- If you add the same item again, its quantity just increases in the cart
- You can return some or all of an item from the cart
- Checkout prints the bill with the total
- If you type something wrong it shows a message and doesnt crash

## How to run

1. Open the notebook in jupyter (or vscode)
2. Run the first cell, it has all the items, prices and the empty cart
3. Run the second cell, this starts the menu
4. Type your choice in the box and press enter
5. Choose 4 to quit

If you change something in the first cell, run it again before the second one.

## Menu

```
What Do you want to do?
1) Shop
2) Return Something
3) Checkout
4) Quit
```

1) Shop - pick a category, then the item, then how many you want. Press 5 in the category menu or 0 in the item menu to go back.

2) Return Something - shows whatever is in your cart and you pick what to return and how many. If you return all of it, the item is removed.

3) Checkout - prints the bill and total, then asks if you want to pay. If you type y the cart is cleared, if you type anything else the cart stays.

4) Quit - ends the program

## Items and prices

Electronics: Phone 5, Laptop 7, Headphones 4, Earbuds 8

Fruits and Vegetables: Apples 7, Banana 8, Watermelon 2, Mango 12

Groceries: Bread 5, Flour 9, Juice 4, Paneer 8

Self Care: Shampoo 6, Conditioner 6, Face Wash 9

## Example bill

```
      BILL
Apples : Rs 7 x 2 = Rs 14
Bread : Rs 5 x 2 = Rs 10

Total = Rs 24
Pay now? (y/n): y
Payment done. Thank you for shopping!
```

## What I used

dictionaries, lists, while and for loops, if/elif/else, break and continue, input(), isdigit(), int() and del

Each category is a dictionary (item name : price) and the 4 dictionaries are kept in a list called Supermarket. The cart is also a dictionary, like this:

```python
cart={'Apples':[7, 3], 'Bread':[5, 2]}
```

Here 7 is the price and 3 is the quantity.

## Problems / things to add later

- The cart is lost if you restart the notebook because nothing is saved in a file
- To add a new item you have to edit the first cell
- No stock, discount or tax right now
- Can use functions to make the code shorter once we learn them
