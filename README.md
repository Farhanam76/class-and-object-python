# class-and-object-python
# tutorial 
class Student:

    def __init__(self, name, age):
        self.name = name
        self.age = age
 John = Student("John", "21")
Jane = Student("Jane", "22")       
print(getattr(John, "age"))
#exercise 

class Student:
    name = "Bob"

    def age(self):
        print("22")

    def classyear(self):
        print("2020")

bob = Student()
print(bob.name)
bob.age()
bob.classyear()

#with init
class Student:
    def __init__(self, name, age, classyear):
        self.name = name
        self.age = age
        self.classyear = classyear

bob = Student("Bob", "22", "2020")

print(bob.name)
print(bob.age)
print(bob.classyear)

# accounts
class Budgets:
    def __init__(self, balance):
        self.balance = balance

    def deposit(self, deposit):
        self.balance += deposit

    def withdraw(self, withdrew):
        self.balance -= withdrew


food_budget = Budgets(1)
food_budget.deposit(20)
food_budget.withdraw(5)

clothes_budget = Budgets(0)
clothes_budget.deposit(500)
clothes_budget.withdraw(7000)

print("Food budget Balance:", food_budget.balance)
print("Clothes budget Balance:", clothes_budget.balance)

