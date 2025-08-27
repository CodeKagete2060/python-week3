# 🧮 Discount Calculator (Python Assignment)

## 📌 Overview
This is a simple Python program that calculates the final price of an item after applying a discount.  

The program:
- Defines a function `calculate_discount(price, discount_percent)`.
- Applies the discount **only if it is 20% or higher**.
- Otherwise, it returns the original price.
- Prompts the user to enter the **original price** and the **discount percentage**.
- Prints the final price after calculation.

---

## 🛠 How It Works
1. The user enters the original price of the item.
2. The user enters the discount percentage.
3. The program checks:
   - ✅ If discount is **20% or more**, it applies the discount.  
   - ❌ If discount is less than 20%, the price remains the same.
4. The final result is displayed.

---

## 📜 Function Definition
```python
def calculate_discount(price, discount_percent):
    if discount_percent >= 20:
        discount_amount = (discount_percent / 100) * price
        final_price = price - discount_amount
        return final_price
    else:
        return price
