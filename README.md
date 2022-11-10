# fracciones
#Clase
class Fraction():
    #Atributos#
    numerator = 0
    denominator = 0
    #Fin Atributos#

    #Constructor#
    def __init__(self,numerator,denominator):
        self.numerator = numerator
        self.denominator = denominator
    #Fin Constructor#



    #Metodos#
    def multiplication(self,a1):
        numerator = self.numerator * a1.numerator
        denominator = self.denominator * a1.denominator
        print("\nEl resultado de la multiplicacion:",numerator,"/",denominator)

    def division(self,a1):
        numerator = self.numerator * a1.denominator
        denominator = self.denominator *a1.numerator
        print("\nEl resultado de la division:",numerator,"/",denominator)

    def addition(self,a1):
        if(self.denominator != a1.denominator):
            denominator = self.denominator * a1.denominator
            numerator = (self.numerator*a1.denominator)+(a1.numerator*self.denominator)
            print("\nEl resultado de la suma:",numerator,"/",denominator)
        else:
            numerator = self.numerator + a1.numerator
            print("\nEl resultado de la suma:",numerator,"/",self.denominator)

    def subtraction(self,a1:
        if(self.denominator != a1.denominator):
            denominator = self.denominator * a1.denominator
            numerator = (self.numerator*a1.denominator)-(a1.numerator*self.denominator)
            print("\nEl resultado de la resta:",numerator,"/",denominator)
        else:
            numerator = self.numerator - a1.numerator
            print("\nEl resultado de la resta:",numerator,"/",self.denominator)

#Iniciar variables
numerator_1 = 0
numerator_2 = 0
denominator_1 = 0
denominator_2 = 0
frac_1 = 0
frac_2 = 0
opcion = 0



#Ingreso de datos
numerator_1 = int(input("Numerador fraccion A: "))
while(denominator_1 == 0):
    denominator_1 = int(input("Denomiandor fraccion A: "))
    if(denominator_1!=0):
    
numerator_2 = int(input("Numerador fraccion B: "))
while(denominator_2 == 0):
    denominator_2 = int(input("Denominador fraccion B: "))
    if(denominator_2!=0):

#Variables
frac_1 = Fraction(numerator_1, denominator_1)
print("Fraccion A =",frac_1.numerator,"/",frac_1.denominator)
frac_2 = Fraction(numerator_2, denominator_2)
print("Fraccion B =",frac_2.numerator,"/",frac_2.denominator)
#Menus
print("\n----FRACCIONES-----\n")
print("MULTIPLICACION(*)")
print("DIVISION(/)")
print("SUMA(+)")
print("RESTA(-)\n")
print("---------------------------------------------------------\n")
opcion = input("Ingrese el simbolo correspondiente a la operacion matematica que quiera (* / + -):")

match(opcion):
    case '+':
        frac_1.multiplication(frac2)
    case '-':
        frac_1.division(frac_2)
    case '*':
        frac_1.addition(frac_2)
    case '/':
        frac_1.subtraction(frac_2)
