# oops-task

1. class Vehicle:

    def __init__(self, name, max_speed, mileage):
        self.name = name
        self.max_speed = max_speed
        self.mileage = mileage

class Van(Vehicle):
    pass

School_van = Van("School Volvo", 180, 30)
print("Vehicle Name:", School_van.name, "Speed:", School_van.max_speed, "Mileage:", School_van.mileage)


2. class Vehicle:
    def __init__(self, capacity):
        self.capacity = capacity

    def fare(self):
        return self.capacity * 10

class Van(Vehicle):
    pass

School_van = Van("5")
print("Total Van fare is:", School_van.fare())


3. When a class is derived from more than one base class it is called multiple Inheritance. The derived class inherits all the features of the base case.


4. class Class1:
	def m(self):
		print("In Class1")
	
class Class2(Class1):
	def m(self):
		print("In Class2")

class Class3(Class1):
	def m(self):
		print("In Class3")
		
class Class4(Class2, Class3):
	pass
	
obj = Class4()
obj.m()



5. Getter: A method that allows you to access an attribute in a given class. 
Setter: A method that allows you to set or mutate the value of an attribute in a class.



6. class Geek:
    def __init__(self, age = 0):
         self._age = age
      
    def get_age(self):
        return self._age
      
    def set_age(self, x):
        self._age = x
  
     raj = Geek()
  
 raj.set_age(21)
  
 print(raj.get_age())
  
    print(raj._age)


7. Method overriding is an ability of any object-oriented programming language that allows a subclass or child class to provide a specific implementation of a method that is already provided by one of its super-classes or parent classes.



8. class Parent():
	
	
	def __init__(self):
		self.value = "Inside Parent"
		
	
	def show(self):
		print(self.value)
		

class Child(Parent):
	
	
	def __init__(self):
		self.value = "Inside Child"
		
	
	def show(self):
		print(self.value)
		
		
obj1 = Parent()
obj2 = Child()

obj1.show()
obj2.show()
