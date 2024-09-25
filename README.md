# act5_programa_que_almacene_un_numero

print("")
print("MARTINEZ TAGLE LUIS ANGEL 3W")
print("")

print("PROGRAMA QUE ALMACENA UN NUMERO")

import random


def main():
    """
    
    Programa que genera un número aleatorio y permite al usuario adivinarlo.
    El usuario recibe pistas sobre si su suposición es demasiado alta o baja.
    """
   
    # Generar un número aleatorio entre 1 y 20
    numero_secreto = random.randint(1, 20)
    intentos = 0  # Contador de intentos del usuario

   
    print("Bienvenido al juego de adivinar el número.") #imprime la bienvenida
   
    print("He seleccionado un número entre 1 y 20. ¡Intenta adivinarlo!") #imprime el mensaje 

   
    while True:
       
        try:
            
            # Solicitar al usuario que ingrese un número
            suposicion = int(input("Introduce tu suposición: "))
            intentos += 1  # Incrementar el contador de intentos

           
            # Comparar la suposición del usuario con el número secreto
           
            if suposicion < numero_secreto:
                print("Demasiado bajo. Intenta de nuevo.")
            
            elif suposicion > numero_secreto:
                print("Demasiado alto. Intenta de nuevo.")
            
            else:
                
                print(f"¡Correcto! Has adivinado el número {numero_secreto} en {intentos} intentos.")
                break  # Salir del bucle si el usuario adivina correctamente

       
        except ValueError:
            
            # Manejo de errores si la entrada no es un número válido
            print("Por favor, introduce un número entero válido.")


if __name__ == "__main__":
main()  # Ejecutar la función principal

   ![image](https://github.com/user-attachments/assets/871ca6f6-3c32-4caf-b7db-19e4cf8f9330)



  ![image](https://github.com/user-attachments/assets/a649b2cd-f4fd-4df6-ae38-14d095f37b04)



