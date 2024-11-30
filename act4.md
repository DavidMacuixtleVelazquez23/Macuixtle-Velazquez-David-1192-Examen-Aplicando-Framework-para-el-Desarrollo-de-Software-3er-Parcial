print("\nMacuixtle Velazquez David\n") 
class Calculadora(): #aqui se declara una clase
    def __init__(self, num1, num2):
        self._num1=num1 
        self._num2=num2
#aqui se declara varias funciones 
#cada una con su respectivo nombre y parametros
    def suma(self):
        resultado=self._num1 + self._num2
        print(f"El resultado de la suma es: {self._num1} + {self._num2}= {resultado}")

    def resta(self):
        resultado=self._num1 - self._num2
        print(f"El resultado de la resta es: {self._num1} - {self._num2}= {resultado}")

    def division(self):
        resultado=self._num1 // self._num2
        print(f"El resultado de la divisón es: {self._num1} // {self._num2}= {resultado}")

    def multiplicacion(self):
        resultado=self._num1 * self._num2
        print(f"El resultado de la multiplicación es: {self._num1} * {self._num2} = {resultado}")

#aqui se ingresan algunos datos 
# y se crea un objeto de la clase calculadora
#para dar paso a la ejecucion
operacion=Calculadora(10, 5) 
operacion.suma()

operacion=Calculadora(10, 5) 
operacion.resta()

operacion=Calculadora(10, 5) 
operacion.division()

operacion=Calculadora(10, 5) 
operacion.multiplicacion()

![image](https://github.com/user-attachments/assets/95829e55-5e90-4ae7-bdeb-fa9cf07c8257)

![image](https://github.com/user-attachments/assets/2291b915-0098-4479-9904-5a3e63d35142)
