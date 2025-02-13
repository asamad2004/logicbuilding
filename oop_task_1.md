## what is class ? ##
1. It is a blueprint for the object it have methods or we can say behavior for the opcoming object.
2. With the help of class we can write real world problems in programming format.
3. We can bind the data with the help of class. 

## what is an object ? ##
1. It is an implimentation of the class
2. It have attributes .
3. We can call methods in the object.

   Question? for calling the object method we need to use (.) operator why we are using this can we call it like this:- object(method)

## what is attribute ? ##
1. It holds values of an object.

## what is method ? ##
1. it is like function that are used in objects.

   Question? if i have to perform addition in the programm then why are we making methods in the class, instead of doing this we can just call the function which i made earlier in the programm? it dosen't take space.

## constructor ##
   we use constructor for initializing object, it allocates memory to the object.
   Keyword :- __init__

## self keyword ##

   It gives you the refrence of current instance.

## code example of class, with object, parameters and methods  ##      
```
class drink:

    def __init__(self, coldrink, whisky, shampane):
        self.coldrink = coldrink
        self.whisky = whisky
        self.shampane = shampane

    def withoutice(self):
        print(f"The drink {self.coldrink} is ready")

    def withice(self):
        print(f"The drink {self.whisky} is ready")    

drink_1 = drink("cola","old monk", "godawan")
drink_1.withoutice()
```