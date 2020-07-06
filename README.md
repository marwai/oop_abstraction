### Abstraction
* Process of hiding the real implementation of an application from the user and emphasising only the usage of it. For example, 
consider a electronic gadget with instruction of the application. The user guide has instructions on how to use the gadget 
but but no information regarding the internal working of the gadget
* A programmer can hide all the irrelevant data/processes of an application to reduce complexity and increase efficiency
* An abstract class cannot be instantiated, i.e.,objects cannot be created for the abstract class.
```
from abc import ABC  # import the abstract class module


class Polygon(ABC):  # sets the abstract class for the other classes to take
    def noofsides(self):
        pass


class Triangle(Polygon):  # overrides the method in the Polygon class
    def noofsides(self):
        print("I have 3 sides")


class Square(Polygon):  # overrides the method in the Polygon class
    def noofsides(self):
        print("I have 4 sides")

#  BC works by decorating methods of the base class as abstract and then registering concrete classes as implementations
 of the abstract base. 
```
