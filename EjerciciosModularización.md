**Ejercicio 1301:**

&#x20;

&#x20;# funciones.py:



def prueba(x,y):



&#x20;**"""**

&#x20;Se define una nueva función (con la palabra def) llamada prueba, x-y son

&#x20;parámetros formales que comunican la función con la parte quela invoca

&#x20;**"""**



&#x20;print(a,b)

&#x20;x = x + 1

&#x20;y = y + 2



**"""**

&#x20;Se muestran en pantalla los valores de a y b. Luego se aumenta uno al valor de X y se aumenta 2 al valor de Y.

**"""**



&#x20;return(x,y)



**"""**

Se devuelve los valores de X,Y 

**"""**





\# programa.py



from funciones import \*



**"""**

Se importan las funciones que están dentro del modulo funciones.py

**"""**



a = int(input("Ingrese un número entero: "))

b = int(input("Ingrese un número entero: "))



**"""**

Se pide ingresar un valor para a y b, que se convierte en entero.

"""



for i in range(3):

&#x20;   print(prueba(a,b))

&#x20;   a = a + 2

&#x20;   b = b + 2



**"""**

Se inicia una estructura de repetición, en este caso se repite el bloque de abajo 3 veces. lo que va a hacer que a los valores a y b se le aumente 2 en cada repetición.

**"""**





**Ejercicio 1302**:



\# funciones.py

def prueba(a,b):

&#x20;   a = a + 1

&#x20;   b = b + 2

&#x20;   return(a,b)



"""

Se define una función llamada prueba que recibe los parámetros a y b. Luego se incrementa el valor de a en 1 y el valor de b en 2, y se guarda el nuevo valor. Por ultimo devuelve los valores mediante return.



"""



\# programa.py:

from funciones import \*



a = int(input("Ingrese un numero entero: "))

b = int(input("Ingrese un numero entero: "))

for i in range(3):

&#x20;   a, b = (prueba(a,b))

&#x20;   a = a + 2 

&#x20;   b = b + 2



**"""**

Primero se utilizan las funciones del modulo funciones.py, luego pide ingresar dos números enteros que se guardan en a y b. Se inicia un ciclo for que se repite tres veces , se llama a la función prueba para utilizar los valores ingresados de a y b , después se repite el  código de bloque en donde se le suma dos valores en a y dos valores a b.



**"""**



**PREGUNTA:** ¿Con qué valores quedan las variables a y b luego de ejecutar el siguiente programa, si ingresamos como datos a=2 y b=3?

. Los valores con los que queda son: a=11 b=15, ya que al inicial el ciclo for se va a repetir 3 veces el bloque de código del programa principal y también el de la función prueba, por lo tanto en cada vuelta a aumenta 3 y b aumenta 4.  





**Ejercicio 1303:** 



&#x20;# funciones.py

&#x20;def valifar\_dni(dni):

&#x20;    cantidad = 0    



**"""**

Primero se define una función llamada validar\_dni en donde se recibe un parámetro que es DNI, luego se inicia una variable cantidad en cero.

**"""**



&#x20;    while dni ¡= 0:

&#x20;          cantidad = cantidad + 1

&#x20;          dni = dni // 10

&#x20;    return cantidad == 8



**"""**

&#x20;Se inicia un ciclo de repetición while que se va a repetir mientras DNI sea distinto a 0, luego cada vez que el ciclo se repite se suma 1 a cantidad. 

Se realiza una división entera a DNI en donde se le elimina el ultimo digito, esto se repite hasta llegar a 0. Fusiona para comprobar que el DNI tiene 8 dígitos, la ultima linea te devuelve true si la cantidad de dígitos es 8 y false si es diferente.



**"""** 



&#x20;# programa.py:

&#x20;from funciones import \*

&#x20;mayor =- 1

&#x20;dni = int(input("DNI: "))



**"""**

Se inicia la variable mayor con el valor -1 que guarda el valor mas grande , luego pide ingresar un DNI que se guarda como entero. 



**"""**



&#x20;while dni ¡= 0.

&#x20;     if validar\_dni(dni):

&#x20;        nombre = input("Nombre: ")

&#x20;        edad = int(input("Edad: "))

&#x20;        if edad > mayor:

&#x20;           mayor = edad

&#x20;           nmbre\_mayor = nombre

&#x20;       

&#x20;     else:

&#x20;         print("DNI invalido. vuelva a ingresar.")

&#x20;      dni = int(input("DNI: "))

&#x20;   print("Nombre de la persona mayor: ", nombre\_mayor) 



**"""**

Se inicia un ciclo while que se repite mientras en DNI sea distinto a 0, luego se inicia una estructura condicional con la función validar\_dni (solo si el DNI es de 8 dígitos) se pide ingresar nombre y edad (se guarda como entero) y si la edad es mayor al valor guardado en la variable MAYOR se actualizan las variables mayor y nombre\_mayor. 

Si el DNI es invalido, se muestra un mensaje de error y se pide ingresar otro DNI.

Por ultimo se imprime el nombre guardado en la variable nombre\_mayor



**"""**



**Pregunta:** ¿Cuál es el resultado de ejecutar el programa anterior con los datos proporcionados en el ejemplo de entrada?



34567890

María Giménez

18



28907678

Carlos Alberto Sánchez

21



0



**Respuesta:** El programa va a devolver Carlos Alberto Sánchez, cuando se ingresa el número 0 se para el ciclo por lo tanto se va a mostrar el nombre Carlos ya que la variable mayor guarda el valor más grande, en este caso la edad de Carlos 

&#x20;. El programa va a devolver error o "DNI inválido. Vuelva a ingresar." ya que el DNI tiene 9 dígitos 





**Ejercicio 1304:** 

&#x20;

El programa que funciona es la opción 3

&#x20;. La opción 1 es incorrecta y salta error ya que no utiliza parámetros, se crean en el programa principal pero la función esta definida en funciones 

&#x20;. El error en la opción 2 es que utiliza como paramentos x, y pero al momento de imprimirlos utiliza a y b, que no están definidas 











&#x20;  



