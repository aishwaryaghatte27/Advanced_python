class CreditCard:
    def pay(self, amount):
        print("Paid ₹", amount, "using Credit Card")


class UPI:
    def pay(self, amount):
        print("Paid ₹", amount, "using UPI")


class PayPal:
    def pay(self, amount):
        print("Paid ₹", amount, "using PayPal")


# Payment Processor

class PaymentProcessor:
    def __init__(self, strategy):
        self.strategy = strategy

    def make_payment(self, amount):
        self.strategy.pay(amount)


# Main program

print("1. Credit Card")
print("2. UPI")
print("3. PayPal")

choice = int(input("Choose payment method: "))
amount = float(input("Enter amount: "))

if choice == 1:
    processor = PaymentProcessor(CreditCard())
elif choice == 2:
    processor = PaymentProcessor(UPI())
elif choice == 3:
    processor = PaymentProcessor(PayPal())
else:
    print("Invalid choice")
    exit()

processor.make_payment(amount)
