# wk3.py

#Week 3 assignment

def calculate_discount(price, discount_percent):
    if discount_percent >= 20:
        discount_price = (discount_percent / 100) * price
        final_price = price - discount_price
        return final_price
    return price

try:
    price = float(input("Enter original price: "))
    discount_percent = float(input("Enter discount percentage: "))

    final_price = calculate_discount(price, discount_percent)
    print(f"The final price is: {final_price:.2f}")
except ValueError:
    print("Invalid input. Please enter numeric values.")
