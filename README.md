# Credit-Union-Account
class BankAccount:
    def __init__(self, account_number, initial_balance):
        self.account_number = account_number
        self._balance = initial_balance

    @property
    def balance(self):
        return self._balance

    def deposit(self, amount):
        self._balance += amount

    def withdraw(self, amount):
        self._balance -= amount

    @property
    def is_overdrawn(self):
        return self._balance < 0

account = BankAccount("123456", 100)
print(f"Initial balance: {account.balance}")

account.deposit(50)
print(f"Balance after deposit: {account.balance}")

account.withdraw(200)
print(f"Balance after withdrawal: {account.balance}")
