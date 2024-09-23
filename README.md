# Reto_13
>#### 1.Desarrollar un algoritmo que imprima de manera ascendente los valores (todos del mismo tipo) de un diccionario.
```python
valores = list(dic1.values()) # Obtener los valores del diccionario en una lista
valores.sort(reverse=True)  # Ordenar los valores
for valor in valores: # Recorrer los valores
    print(valor) # Imprimir los valores ordenados
```
>#### 2.Desarrollar una funcion que reciba dos diccionarios como parametros y los mezcle, es decir, que se construya un nuevo diccionario con las llaves de los dos diccionarios; si hay una clave repetida en ambos diccionarios, se debe asignar el valor que tenga la clave en el primer diccionario.
```python
def mezclar_dic(dic1, dic2):
  dic_mezclado = dic2.copy()  # Copiamos el segundo diccionario
  dic_mezclado.update(dic1)   # Actualizamos con los valores del primer diccionario
  return dic_mezclado
```
>#### 3,Cree un programa que lea de un archivo con dicho JSON y:Imprima los nombres completos (nombre y apellidos) de las personas que practican el deporte ingresado por el usuario. Imprima los nombres completos (nombre y apellidos) de las personas que est�en en un rango de edades dado por el usuario.
```python
def personas_por_deporte(deporte_ingresado):
  print(f"Personas que practican {deporte_ingresado}:")
  for persona in personas.values():
    if deporte_ingresado in persona["deportes"]:
      print(f"{persona['nombres']} {persona['apellidos']}")

def imprimir_personas_por_edad(rango_minimo, rango_maximo):
  print(f"Personas entre {rango_minimo} y {rango_maximo} años:")
  for persona in personas.values():
    if rango_minimo <= persona["edad"] <= rango_maximo:
      print(f"{persona['nombres']} {persona['apellidos']}")
```
