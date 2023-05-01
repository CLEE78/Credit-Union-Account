# Credit-Union-Account
class BankAccount:
    def __init__(self, account_number, initial_balance):
        self.account number = account_number
        self.balance = initial_balance


    def balance(self):
        return self.balance

    def deposit(self, amount):
        self.balance += amount

    def withdraw(self, amount):
        self.balance -= amount

   
    def is_overdrawn(self):
        return self.balance < 0

account = BankAccount("123456", 100)
print(f"Initial balance: {account.balance}")

account.deposit(50)
print(f"Balance after deposit: {account.balance}")

account.withdraw(200)
print(f"Balance after withdrawal: {account.balance}")
