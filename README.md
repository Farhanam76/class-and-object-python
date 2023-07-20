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
def transfer(self, other_category, amount):
        if amount <= self.balance:
            self.withdraw(amount)
            other_category.deposit(amount)
        else:
            print(" not enough to transfer")


food_budget = Budgets(1)
food_budget.deposit(20)
food_budget.withdraw(5)
food_budget.transfer(clothes_budget, 40)

print("After Transfer:")
clothes_budget = Budgets(0)
clothes_budget.deposit(500)
clothes_budget.withdraw(7000)

print("Food budget Balance:", food_budget.balance)
print("Clothes budget Balance:", clothes_budget.balance)


#files tutorial: 
file = open("pyproject.toml", "r")

outfile = ""

for line in range(1, 10):
    if line % 2 == 0:
        outfile += file.readline()
    else:
        file.readline()

file.close()

file = open("filename.txt", "w")
file.write(outfile)
file.close()

with open("pyproject.toml","r") as file: 
  information = file.read()

print(information)

1. Write a Python program to read an entire text file.
file = open("pyproject.toml", "r")
line = file.readlines()
print(lines)
file.close()

