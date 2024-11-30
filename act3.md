print("\nMacuixtle Velazquez David\n")
class triangulo: #aqui se declara una clsse 
    def __init__(self,lado1,lado2,base):
        self.lado1 = lado1
        self.lado2 = lado2
        self.base = base

    def calcular_area(self): #aqui se declara una funcion
        #despues se inicia una secuencia if para saber que tipo de triangulo es
        if self.lado1 == self.lado2 == self.base:
            print("El triangulo es equilátero")
        if self.lado1 == self.lado2 != self.base:
            print("El triangulo es isósceles")
        if self.lado1 != self.lado2 != self.base:
            print("El triangulo es escaleno")
#aqui se pide al usuario que ingrese los datos para crear un objeto de la clase triangulo
lado1 = float(input("Ingrese el valor del lado 1: "))
lado2 = float(input("Ingrese el valor del lado 2: "))
base = float(input("Ingrese el valor de la base: "))


p1 = triangulo(lado1,lado2,base)#aqui se crea un objeto de la clase triangulo
p1.calcular_area()#aqui se ejecuta la funcion

![image](https://github.com/user-attachments/assets/26525651-a9f5-4b42-b380-98dab93905be)
![image](https://github.com/user-attachments/assets/51b76523-1e9a-4af7-9aaf-7ed566648ff8)
