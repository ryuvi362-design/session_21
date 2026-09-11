[README_21.md](https://github.com/user-attachments/files/32095100/README_21.md)
```python
class Product:
    def get_discount(self):
        return 0


class Electronics(Product):
    def get_discount(self):
        return 10


product = Product()
electronic = Electronics()

print("Product discount:", product.get_discount(), "%")
print("Electronics discount:", electronic.get_discount(), "%")
```

```python
class FoodOrder:
    def __init__(self, price):
        self.price = price

    def calculate_total(self):
        return self.price


class ZomatoOrder(FoodOrder):
    def calculate_total(self):
        return self.price + (self.price * 0.05)


order = ZomatoOrder(1000)

print("Total price:", order.calculate_total())
```

```python
class Influencer:
    def bonus(self):
        return 2000


class BrandManager:
    def bonus(self):
        return 5000


def show_bonus(employee):
    print("Bonus:", employee.bonus())


influencer = Influencer()
manager = BrandManager()

show_bonus(influencer)
show_bonus(manager)
```

```python
class User:
    def get_status(self):
        return "active"


class PremiumUser(User):
    def get_status(self):
        return "premium"


user = User()
premium_user = PremiumUser()

print("User status:", user.get_status())
print("Premium User status:", premium_user.get_status())
```
