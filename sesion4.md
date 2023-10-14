<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 4

## EJERCICIO 1 ##

def calculadora(n1,n2,op):
    resultado = 0
    if op == '+':
        resultado = n1 + n2
    elif op == '-':
        resultado = n1 + n2
    elif op == '*':
        resultado = n1 * n2
    elif op == '/':
        resultado = n1 / n2
    return resultado

#x = calculadora(5,8,"+")
#print(x)

num1 = int(input("Ingrese el primer numero: "))
num2 = int(input("ingrese el segundo numero: "))
op = input("Ingrese el operador: ")
x = calculadora(num1,num2,op)
print(x)

## EJERCICIO 2 ##

def contar_vocales(cadena):
    # Inicializamos un contador de vocales
    contador = 0
    
    # Recorremos cada carácter en la cadena
    for caracter in cadena:
        # Convertimos el carácter a minúsculas para hacer la comparación insensible a mayúsculas/minúsculas
        caracter = caracter.lower()
        
        # Verificamos si el carácter es una vocal
        if caracter in ('a', 'e', 'i', 'o', 'u'):
            contador += 1
    
    return contador

# Ejemplo de uso:
cadena = "Hola, esta es una cadena de ejemplo con vocales."
resultado = contar_vocales(cadena)
print(f"La cadena tiene {resultado} vocales.")

## EJERCICIO 3 ##

def es_primo(numero):
    # Verificar si el número es menor o igual a 1
    if numero <= 1:
        return False
    
    # Si el número es 2 o 3, es primo
    if numero <= 3:
        return True
    
    # Si el número es divisible por 2 o 3, no es primo
    if numero % 2 == 0 or numero % 3 == 0:
        return False
    
    # Comprobar divisibilidad por números impares a partir de 5
    i = 5
    while i * i <= numero:
        if numero % i == 0 or numero % (i + 2) == 0:
            return False
        i += 6
    
    return True

# Ejemplo de uso:
numero = 17
resultado = es_primo(numero)
if resultado:
    print(f"{numero} es un número primo.")
else:
    print(f"{numero} no es un número primo.")

## EJERCICIO 4 ##

def contar_palabras(cadena):
    # Dividir la cadena en palabras utilizando el espacio como delimitador
    palabras = cadena.split()
    
    # Contar la cantidad de palabras
    cantidad_palabras = len(palabras)
    
    return cantidad_palabras

# Ejemplo de uso:
cadena = "Esta es una cadena de ejemplo con varias palabras."
resultado = contar_palabras(cadena)
print(f"La cadena tiene {resultado} palabras.")

## EJERCICIO 5 ##

def potencia(base, exponente):
    # Utilizamos el operador ** para calcular la potencia
    resultado = base ** exponente
    return resultado

# Ejemplo de uso:
base = 2
exponente = 3
resultado = potencia(base, exponente)
print(f"{base} elevado a la potencia {exponente} es igual a {resultado}")

   
<!-- Su documentación aquí -->






