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



  
 
