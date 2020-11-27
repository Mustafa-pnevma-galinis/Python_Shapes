Proeme =                                                       "بسم اللّه الرحمن الرحيم و عليه توكلنا"
# Python_Shapes
class Circle :
    def __init__(self,rad):
        self.rad = rad  # self is like {this} in Java.
    def calcArea (self):
        circArea = math.pow(self.rad,2) * math.pi
        print("Circle Area equals : {}.".format(round(circArea)))
    def calcPerimeter(self):
        circPerimeter = 2 * self.rad * math.pi
        print("Circle Perimeter equals: {}.".format(round(circPerimeter)))
#x = Circle (int(input("Enter your desired num: "))) #Object
               #Equalise variable <x> to the class which indicates a constructor or initialiser;
               #with a value of {radius} in this example..
        #Note: The class is initialised with variable {rad}...
        #Note: we initialise a variable in (__init__) method instead of iterating it in each method..
        #      so this variable is utilisable in each method under the class.


class Square :
    def __init__ (self , length):
        self.length = length
    def calcArea(self):
        sqrArea = math.pow(self.length , 2)
        print(f"Square Area = {sqrArea}")
    def calcPerimeter (self):
        sqrPerimeter = 4 * self.length
        print(f"Square Perimeter = {sqrPerimeter}")

favShape = input ("Enter your favourite shape {Circle / Square} : ")
if favShape == "Circle" :
    x = Circle (int(input("Enter a num : ")))
    interCalc = input ("Area / Perimeter : ")
    if interCalc == "Area" :
        x.calcArea()
    elif interCalc == "Perimeter":
        x.calcPerimeter()
elif favShape == "Square" :
    y = Square (int(input("Enter a num: ")))
    interCalc = input ("Area / Perimeter : ")
    if interCalc == "Area" :
        y.calcArea()
    elif interCalc == "Perimeter" :
        y.calcPerimeter()
