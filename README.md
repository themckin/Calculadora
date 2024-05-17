#Calculadora completa

def Sumar(num_1,num_2):
    return num_1 + num_2

def resta (num_1,num_2):
    return num_1 - num_2
   
def multi (num_1,num_2):
    return num_1 * num_2

def division (num_1,num_2):
    if num_2 != 0:
        return num_1 / num_2
    else:
        return "Error: operacion no permitida"

print("Seleccione la operación:") 
print("1. Suma") 
print("2. Resta") 
print("3. Multiplicacion") 
print("4. Dividision")

operacion = input("Ingresa el numero de la operacion que desea: (1/2/3/4)")


num_1 = int(input("ingresa un numero: "))
num_2 = int(input("ingresa otro numero: "))

if operacion == "1":
    resultado = Sumar(num_1,num_2)
    print(f"el resultado de la suma es : {resultado}")
    
elif operacion == "2":
    resultado = resta (num_1,num_2)
    print(f"el resultado de la resta es : {resultado}")

elif operacion == "3":
    resultado = multi (num_1,num_2)
    print(f"el resultado de la multiplicacion es : {resultado}")
    
elif operacion == "4":
    resultado = division (num_1,num_2)
    print(f"el resultado de la division es : {resultado}")
    
else:
    print("Error operacion no valida en el sistema
