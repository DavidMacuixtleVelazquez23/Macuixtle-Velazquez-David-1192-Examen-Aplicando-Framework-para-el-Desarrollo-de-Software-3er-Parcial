
print("\n2- Mostrar Contacto\n")
nose = int(input("Escribe un número: "))  # Pedir al usuario que elija una opción

if nose == 2:
    # Definimos la clase Contacto
    class Contacto:
        def __init__(self, nombre, telefono):
            self.nombre = nombre  # Nombre del contacto
            self.telefono = telefono  # Teléfono del contacto

        # Método para mostrar los detalles del contacto
        def mostrar(self):
            print(f"Nombre: {self.nombre}, Teléfono: {self.telefono}")

        # Método para buscar un nombre en una lista predefinida
        def nosea(self):
            lista = ["Zoe", "Juan", "Manolo"]  # Lista de nombres
            resp = input("Escriba el nombre: ")  # Nombre a buscar
            if resp in lista:
                print(f"Yes, '{resp}' está en la lista")
            else:
                print(f"No, '{resp}' no está en la lista")

        # Método para cambiar el nombre del contacto
        def cambiar(self, nuevo_nombre):
            print(f"El nombre del contacto '{self.nombre}' ha sido cambiado a '{nuevo_nombre}'.")
            self.nombre = nuevo_nombre  # Actualizar el nombre del contacto

    # Lista para almacenar los contactos
    contactos = [
        Contacto("Juan", 123456),
        Contacto("Manolo", 5325325),
        Contacto("Zoe", 14343144)
    ]

    # Función para mostrar todos los contactos
    def mostrar_contactos():
        print("\nContactos:")
        for idx, contacto in enumerate(contactos):
            print(f"{idx + 1}.", end=" ")
            contacto.mostrar()

    # Función para agregar un nuevo contacto
    def agregar_contacto():
        print("\nAgregar un nuevo contacto:")
        nombre = input("Escriba el nombre del nuevo contacto: ")  # Pedir nombre
        telefono = input("Escriba el teléfono del nuevo contacto: ")  # Pedir teléfono
        contactos.append(Contacto(nombre, telefono))  # Crear y agregar el nuevo contacto
        print(f"Contacto '{nombre}' agregado con éxito.")

    # Mostrar contactos iniciales
    mostrar_contactos()

    # Buscar un nombre en la lista
    contactos[0].nosea()

    # Preguntar al usuario si quiere cambiar un nombre
    print("\n¿Desea cambiar el nombre de un contacto?")
    respuesta = input("Escriba 'sí' para cambiar un nombre: ").lower()
    if respuesta == "sí":
        # Mostrar opciones de contactos
        mostrar_contactos()
        opcion = int(input("Escriba el número del contacto que desea cambiar: "))
        nuevo_nombre = input("Escriba el nuevo nombre: ")  # Pedir el nuevo nombre

        # Cambiar el nombre según la opción seleccionada
        if 1 <= opcion <= len(contactos):
            contactos[opcion - 1].cambiar(nuevo_nombre)
        else:
            print("Opción no válida.")

    # Preguntar al usuario si desea agregar un nuevo contacto
    print("\n¿Desea agregar un nuevo contacto?")
    respuesta_agregar = input("Escriba 'sí' para agregar un contacto: ").lower()
    if respuesta_agregar == "sí":
        agregar_contacto()

    # Mostrar la lista de contactos actualizada
    mostrar_contactos()

if nose == 5:
    # Opción para salir del programa
    print("¿Seguro que desea terminar la ejecución?")
    nose2 = int(input("1-Sí: "))
    if nose2 == 1:
        print("La ejecución se ha detenido.")

![image](https://github.com/user-attachments/assets/2cacf7a5-5c3a-4c54-be5d-5e52794da4ff)
![image](https://github.com/user-attachments/assets/2a54dafc-81b2-432b-a083-7ea621196759)

![image](https://github.com/user-attachments/assets/b236b357-8042-4758-b630-83bc7e7a0e5d)
![image](https://github.com/user-attachments/assets/33688ceb-ff81-4503-b342-d8e01d72c30f)

