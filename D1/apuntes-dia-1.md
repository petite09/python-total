# Apuntes Día 1

Python es un _lenguaje de programación_ (como aprender un nuevo idioma).

Pycharm es un IDE: _entorno de desarrollo integrado_ (_**IDE**_). Es una aplicación de software que ayuda a los programadores a desarrollar código de software de manera eficiente.

Instalación de Python y Pycharm.

---
## 1. Declaración Print

print = imprimir (mostrar en pantalla). Declaración que al ejecutarse muestra (o imprime) en pantalla el argumento que se introduce dentro de los paréntesis.

Comenzando a escribir:

``` python
print("Hola Mundo")
print(123)
```

La palabra clave es **print()** + dentro del paréntesis va lo que queremos que imprima:

- Si es texto, va entre comillas (simples o dobles) **print**(”Hola mundo”) o **print**(’Hola mundo’)
- Si son números u otras funciones, van sin comillas **print**(1234)

Palabras **claves** se ven en **azul**.

**Paréntesis** (en Pycharm) se ven **amarillos**, para poder identificar fácilmente dónde empieza y dónde termina el contenido de print en este caso.

El **texto** ingresado se ve **verde**.

Luego hay que ejecutar el programa: ir a la pestaña “Run” . La otra opción es apretar el triángulo verde en la esquina superior derecha.

Si se quiere poner un texto con comillas al interior del paréntesis de la declaración **print**() es necesario usar otras comillas:

- Si dice **print**(”Hola mundo, te digo ‘Hola’”) con comillas dobles para delimitar lo que está dentro del paréntesis, se debe usar las comillas simples para especificar el texto que quiero que aparezca entre comillas.
- Si dice **print**(’Hola mundo, te digo “Hola”’) ocurre al revés si se usan las comillas simples para definir lo que está dentro del paréntesis.

También se pueden imprimir operaciones:

``` python
print(100+50) # se va a mostrar el resultado: 150 

print("100+50") # si se pone comillas a la operación, se mostrará el 100+50 (se interpreta como texto) 
```

## 2. Strings

En Python existen muchos tipos de datos.

>[!info] Strings
>Los strings en Python son un tipo de dato formado por cadenas (o secuencias) de caracteres de cualquier tipo, formando un texto.

Todo lo que haya en un string será tratado como texto: espacios en blanco, signos especiales, puntuación y hasta operadores matemáticos y números que mientras se encuentren dentro de las comillas no serán tratados matemáticamente.

Los string no solamente se pueden escribir como una sucesión de caracteres como hemos visto hasta ahora, sino que también como varias sucesiones de caracteres y juntarlas o unirlas en lo que llamamos una concatenación.

```python
print('Fede')
print("Hola" + 'Fede') #al ejecutar esto, aparece HolaFede (todo junto)

#Esto se puede arreglar de 3 formas

print("Hola " + 'Fede') o print("Hola" + ' Fede') o print("Hola" + " " + 'Fede') 
#Cada cosa que está entre comillas se considera como una "cadena" (string)

#Uso de la barra invertida \ le estás diciendo al código que el siguiente 
#carácter no va a ser tomado como carácter, sino que es una función especial o 
#un carácter textual.

print("Me llamo \"Federico\"")
```

Cómo escribir dos líneas seguidas con una misma orden print?

```python
print("Esta es una lineaY esta es otra linea")
print("Esta es una linea\\nY Estas es otra linea") #\n indica nueva línea
```

Cuando queremos escribir en inglés:

```python
print('This isnt a number') # isn't se escribe con una comilla y quedaría así
print('This isn't a number') # lo que tiraría un error

# una opción es poner comillas dobles fuera:
print("This isn't a number")

#otra opción es usar la barra invertida \\
print('This ins\\'t a number') #ojo que es solo el carácter siguiente 
```

```python
# qué pasa si queremos escribir una barra invertida \\ en el interior del paréntesis
print('Este signo \\ es una barra invertida') 
# en PyCharm esto lo toma como error, porque la \\ es un carácter de escape
# para solucionar esto, hay que poner otra barra invertida

print('Este signo \\\\ es una barra invertida')
```


>[!info] Input:
>Input es una función que permite al usuario introducir información por medio del teclado al ejecutarse, otorgándole una instrucción acerca del ingreso solicitado. El código continuará ejecutándose luego de que el usuario realice una acción.

Queremos que el usuario final del programa que vamos a crear pueda ingresar su propia información → existe una función para pedirle al usuario que escriba algo y luego poder mostrar esa información o almacenarla para poder hacer algo con eso.

```python
input("tu nombre") #palabra clave es input y entre paréntesis va la explicación o pedido para que el usuario entienda qué es lo que se espera que ingrese.

# La explicaicón debe estar entre comillas, dobles o simples, y responde a todas las característias de un string.
```

En esta lección se aprenderá a imprimir la información en pantalla, para eso se utiliza la declaración print y luego input entre paréntesis.

```python
print(input("tu nombre")) # acá lo que se está diciendo es: **imprimir** lo que **ingresen** al pedir el **nombre**
