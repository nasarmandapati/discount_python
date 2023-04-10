# discount_python
items = {
    "Apple": 100,
    "Banana": 50,
    "Orange": 75,
    "Mango": 120
}

discounts = {
    "Apple": 10,
    "Banana": 5,
    "Orange": 8,
    "Mango": 15
}

def calculate_price(item_name, quantity):
    price_per_item = items[item_name]
    discount_percentage = discounts[item_name]
    total_price = price_per_item * quantity
    discounted_price = total_price * (1 - discount_percentage/100)
    return discounted_price

item_name = input("Enter the item name: ")
quantity = int(input("Enter the quantity: "))

total_price = calculate_price(item_name, quantity)
print("The total price after discount is:", total_price)
