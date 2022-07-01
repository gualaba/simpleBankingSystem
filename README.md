##**VeriTran's Code Exercise**

Your mission is to create a simple banking system. Think about your personal bank account experience. When in doubt, go for the simplest solution. You don’t need to create any kind of user interface or make these features available through any server.

The exercise evolves as a sequence of iterations. Try to complete each iteration before reading the next one.

##**Iteration 1: Add the deposit feature**

class Account():
  def __init__(self, account_id, client_id, balance = 100):
    self.account_id = account_id
    self.client_id = client_id
    self.balance = balance

  def deposit(self, amount):
    self.amount = amount
    self.balance = self.balance + self.amount

  def check_balance(self):
    print("Account balance:", self.balance, "USD")

# Main program

account_id = "f062022"
client_id = "francisco"

account = Account(account_id, client_id)

amount = int(input("Hi " + client_id + ", write the amount to deposit in your account: "))

account.deposit(amount)
account.check_balance()
