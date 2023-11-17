class Animal:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def make_sound(self):
        pass  
        
class Cat(Animal):
    def __init__(self, name, age, color):
        super().__init__(name, age)
        self.color = color

    def make_sound(self):
        return "Meow!"

    def catch_mouse(self):
        return f"{self.name} is catching a mouse!"

class Dog(Animal):
    def __init__(self, name, age, breed):
        super().__init__(name, age)
        self.breed = breed

    def make_sound(self):
        return "Woof!"

    def catch_ball(self):
        return f"{self.name} is catching the ball!"


my_cat = Cat("cookie", 3, "Brown")
my_dog = Dog("bob", 2, "Bulldog")

print(f"{my_cat.name} is {my_cat.age} years old and has {my_cat.color} fur.")
print(f"{my_cat.name} says: {my_cat.make_sound()}")
print(my_cat.catch_mouse())

print(f"{my_dog.name} is {my_dog.age} years old and is a {my_dog.breed}.")
print(f"{my_dog.name} says: {my_dog.make_sound()}")
print(my_dog.catch_ball())

