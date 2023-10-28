1)Explain Class and Object with respect to Object-Oriented Programming. Give a suitable example.

class:-Class is a blueprint which has attributes(properties) and behaviors(methods) that the objects of that class will have.
objects:-objets are variables in python which can be used to store data and functions.


```python
class student:
    def __init__(self,name,marks):
        self.name=name
        self.marks=marks
std=student('siva',90)
print(std.marks)
print(std.name)
```

    90
    siva


in above example student is class and std is object

Q2. Name the four pillars of OOPs.

Four pillers of oops in python are:-
i)Encapsulation
ii)inheritance
iii)polymorphism
iv)abstraction

3)Explain why the __init__() function is used. Give a suitable example.
__init__():-This is a constructor and it is used to initialise the values.it is also called a special method or Dunder method.

```python
class student:
    def __init__(self,name,marks):
        self.name=name
        self.marks=marks
std=student('siva',90)
print(std.marks)
print(std.name)
```

    90
    siva


Q4. Why self is used in OOPs?
self represents instance of a class in python

```python
class students:
    def student(self):
        print("hello everyone")
obj=students()
obj.student()
```

    hello everyone


Q5. What is inheritance? Give an example for each type of inheritance.

Inheritance:-creating of a class which inherits the methods and properties of another class is called inheritance.
types of inheritace:-
i)single imheritance
ii)multiple inheritance
iii)multi level inheritance
iv)hierarchical inheritance


```python
class Animal:
    def anim(self):
        print("animal")
class cat(Animal):
    def sound(self):
        print("meow")
obj=cat()
obj.anim()
obj.sound()
```

    animal
    meow



```python
class Animal:
    def anim(self):
        print("animal")
class Cat(Animal):
    def sound(self):
        print("meow")
class Food(Cat):
    def drinks(self):
        print("cat drinks milk")
obj1=Food()
obj1.anim()
obj1.sound()
obj1.drinks()
```

    animal
    meow
    cat drinks milk



```python
class Animal:
    def anim(self):
        print("animal")
class Cat(Animal):
    def sound(self):
        print("meow")
class Lion(Animal):
    def sound(self):
        print("roar")
Cat_obj=Cat()
Cat_obj.anim()
Cat_obj.sound()
Lion_obj=Lion()
Lion_obj.anim()
Lion_obj.sound()
```

    animal
    meow
    animal
    roar



```python
class subject1:
    def marks1(self):
        print("marks in subject1=",70)
class subject2:
    def marks2(self):
        print("marks in subject2=",90)
class result(subject1,subject2):
    pass
res=result()
res.marks1()
res.marks2()


```

    marks in subject1= 70
    marks in subject2= 90



```python

```
