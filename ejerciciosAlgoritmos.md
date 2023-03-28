# Ejercicios con algoritmos
## Primeros 3 ejercicios

### Ejercicio 1
**Calcular la letra del DNI Español**

**Paso 1**: Definir el problema

¿Cómo se calcula la letra del DNI?

Numero de DNI , que debe tener 8 dígitos, se divide en 23 y el resto es el `resultadoResto`

`resultadoResto` lo compararemos con la lista de códigos de la siguiente tabla de letras ```tablaLetrasDni```



| resultadoResto | Letra |
| -------------- | ----- |
| 0              | T     |
| 1              | R     |
| 2              | W     |
| 3              | A     |
| 4              | G     |
| 5              | M     |
| 6              | Y     |
| 7              | F     |
| 8              | P     |
| 9              | D     |
| 10             | X     |
| 11             | B     |
| 12             | N     |
| 13             | J     |
| 14             | Z     |
| 15             | S     |
| 16             | Q     |
| 17             | V     |
| 18             | H     |
| 19             | L     |
| 20             | C     |
| 21             | K     |
| 22             | E     |

**Paso 2**: Poner la entrada, proceso y salida

Entrada: `DNI y tablaLetrasDNI, resultado`

Proceso: 
- Validar que `DNI` tenga 8 dígitos y que sean todos numéricos

- Si es erróneo, se asigna a la variable `resultado` "DNI Invalido"

- Dividimos `DNI` en 23 y el resto lo asignamos a `resultadoResto`

- Comparar `resultadoResto` con los valores de la tabla `tablaLetrasDNI` y asignamos a `resultado` el valor equivalente en la tabla

Salida: Escribir `resultado`

**Paso 3**: Escribir Pseudocódigo

``` Code Languaje
Algoritmo calculoDNI
	# Entrada
	DNI <- leer()
	tablaLetrasDNI<- "TRWAGMYFPDXBNJZSQVHLCKE"
	resultado <- ""
	# Proceso
	Si DNI es valido Entonces #
		resultadoResto <- DNI mod 23 #mod es el resto de dividir
		# resultado <- recuperarLetra a partir de resultadoResto y tablaLetrasDNI
	Sino
		resultado <-"DNI Inválido"
	Fin Si
	# Salida
	Escribir(resultado)
Fin Algoritmo
```



### Ejercicio 2

**Paso 1**: Definir el problema

**Paso 2**: Poner la entrada, proceso y salida

**Paso 3**: Escribir Pseudocódigo

``` Code Languaje
Algoritmo calculoDNI
	# Entrada
	# Proceso
	# Salida
Fin Algoritmo
```



### Ejercicio 3

**Paso 1**: Definir el problema

**Paso 2**: Poner la entrada, proceso y salida

**Paso 3**: Escribir Pseudocódigo

``` Code Languaje
Algoritmo calculoDNI
	# Entrada
	# Proceso
	# Salida
Fin Algoritmo
```



## Resto de ejercicios

### Ejercicio 4

**Paso 1**: Definir el problema

¿Como calcular área y perímetro de un circulo?

Perímetro es 2xPIxRadio

Área es PIxRadio al cuadrado

**Paso 2**: Poner la entrada, proceso y salida

Entrada: `radio, perimetro, pi, area`

Proceso: - `perimetro` = 2* `pi` * `radio`

- `area` = `pi` * `radio` al cuadrado

**Paso 3**: Escribir Pseudocódigo

``` Code Languaje
Algoritmo calculoAreaPerimetro
	# Entrada
	radio <- valor
	# Proceso
	radioCuadrado <- radio * radio
	
	perimetro <- 2 * 3.14 * radio
	area <- 3.14 * radioCuadrado
	# Salida
	perimetro
	area
Fin Algoritmo
```



### Ejercicio 5

**Paso 1**: Definir el problema

¿Cual es mayor y cual menor?

**Paso 2**: Poner la entrada, proceso y salida

Entrada: `listaNumeros`

Proceso: 

- Validar que la lista es de números

- Asignar a variable `numeroMayor` y `numeroMenor` el primer numero del array

- Comprobar que un numero es mayor o menor que el siguiente con un bucle e ir asignando a `numeroMayor` y `numeroMenor`

- Mostrar `numeroMayor` y `numeroMenor`

Salida:

**Paso 3**: Escribir Pseudocódigo

``` Code Languaje
Algoritmo calculoDNI
	# Entrada
	listaNumeros <- Array
	numeroMayor <- 0
	numeroMenor <- 0
	
	# Proceso
	Si listaNumeros es valido Entonces #
		numeroMayor <- listaNumeros[0]
		numeroMenor <- listaNumeros[0]
		
		Para i=1 Hasta listaNumeros con Paso 1 Hacer
			Si numeroMenor >= listaNumeros[i] Entonces #
				numeroMenor <- listaNumeros[i]
		Fin Para
		
		Para i=1 Hasta listaNumeros con Paso 1 Hacer
			Si numeroMayor <= listaNumeros[i] Entonces #
				numeroMayor <- listaNumeros[i]
		Fin Para
		
	Sino
		"listaNumeros es invalido"
	Fin Si
	
	# Salida
	Mostrar numeroMayor
	Mostrar numeroMenor
	
Fin Algoritmo
```



### Ejercicio 6

**Paso 1**: Definir el problema

¿Como pasar de grados Celsius a Fahrenheit?

Fahrenheit es igual a Celsius x 1.8 + 32

**Paso 2**: Poner la entrada, proceso y salida

Entrada: Asignamos un valor previamente validado a la variable `celsius`

proceso: 

- La variable `faherenheit` es `celsius` * 1.8 + 32

- salida: mostramos `fahrenheit`

**Paso 3**: Escribir Pseudocódigo

``` Code Languaje
Algoritmo FahrenheitCelsius
	# Entrada
	celsius <- leer
	# Proceso
	Si celsius es valido Entonces #
		fahrenheit <- celsius * 1.8 + 32
	Sino
		"El numero es invalido"
	FinSi
	# Salida
	mostrar fahrenheit
Fin Algoritmo
```



### Ejercicio 7

**Paso 1**: Definir el problema

¿Como saber si un numero es par o impar?

Si el numero introducido se divide entre 2 y el resto es 0, es par, sino, es impar.

**Paso 2**: Poner la entrada, proceso y salida

Entrada: Asignamos un valor previamente validado a la variable `numero`

Proceso: 

- Comprobamos si mediante la formula `numero % 2` es 0 u otro numero para ver si es par o impar

Salida: Mostramos si numero es par o impar

**Paso 3**: Escribir Pseudocódigo

``` Code Languaje
Algoritmo parImpar
	# Entrada
	numero <- leer
	par <- True
	# Proceso
	Si numero es valido Entonces #
		Si numero mod 2 es 0
			par <- True
		Sino
			par <- False
	Sino
		"Introduce un numero valido"
	FinSi
	# Salida
	Mostrar par
Fin Algoritmo
```



### Ejercicio 8

**Paso 1**: Definir el problema

¿Como saber si un año es bisiesto?

Un año es bisiesto cuando es divisible entre 4 y su resto es 0

**Paso 2**: Poner la entrada, proceso y salida

Entrada: Asignamos un valor previamente validado a la variable `ano`

Proceso: 

- Comprobamos si `ano` es divisible entre 4 y su resto es 0. Si lo es, es bisiesto

Salida: Mostramos `ano` diciendo si es par o impar

**Paso 3**: Escribir Pseudocódigo

``` Code Languaje
Algoritmo añoBisiesto
	# Entrada
	ano <- leer
	bisiesto <- True
	# Proceso
	Si ano es valido Entonces #
		Si ano mod 4 Entonces #
			bisiesto <- True
		Sino
			bisiesto <- False
	Sino
		"Introduce un numero correcto"
	FinSi
	# Salida
	mostrar bisiesto
Fin Algoritmo
```



### Ejercicio 9

**Paso 1**: Definir el problema

¿Que es una palabra palíndroma? Aquella que se lee igual de ida hacia delante y hacia atrás.

**Paso 2**: Poner la entrada, proceso y salida

Entrada: Asignamos un valor que es una palabra de mínimo 2 letras previamente validado a la variable `palabra`

Proceso:

- Comprobamos dentro de un bucle la primera letra con la ultima letra, la segunda con la penúltima... Si en cada vuelta, la letra es la misma, `palindroma`es `True`, si no, será `False` y saldrá del bucle. Si el bucle termina, la palabra es palíndroma

Salida: mostrar si es palíndroma

**Paso 3**: Escribir Pseudocódigo

``` Code Languaje
Algoritmo palindromo
	# Entrada
	palabra <- leer
	palindroma <- False #Valor aleatorio, puede ser tambien True
	# Proceso
	Si palabra es valido Entonces
		Para i=0 Hasta longitud de palabra con Paso 1 Hacer 
			#len(palabra)
			Si palabra[i] es igual a palabra[-i-1] Entonces
				palindroma <- True
			Sino
				palindroma <- False
				exit
	Sino
		"Escribe una palabra correcta"
	FinSi
	
	# Salida
	mostrar palindroma
Fin Algoritmo


OTRA OPCION

Algoritmo Palindromo
   # Entrada
   cadena <- leer()
   #Proceso
   #cadena <- Convertir a minúsculas y eliminar espacios en blanco
   reversa <- depuracionCadena(cadena)
   Si cadena es igual a reversa entonces
     resultado <- "La cadena es un palíndromo"
   Sino
     resultado <- "La cadena no es un palíndromo"
   Fin Si
   # Salida
   escribir resultado
Fin Algoritmo

SubAlgoritmo depuracionCadena (cadena)
    #quita los espacios en blanco, otros caracteres y convierte todo a minusculas
    i<-0
    Mientras cadena[i] sea diferente de findecadena Haga
        caracter<-""
        Si  el ASCII de cadena[i]  mayor que 64 y ASCII de cadena[i] menor que 91 Entonces
            caracter<-cadena[i] en minusculas
        Fin Si
        Si  el ASCII de cadena[i]  mayor que 96 y ASCII de cadena[i] menor que 123 Entonces
            caracter<-cadena[i]
        End Si
        temporal <- temporal + caracter
        Si caracter es diferente "" Entonces
            i<-i+1
        Fin Si
    Fin Mientras
    L<-i
    reversa<-""
    Para N = 0 Hasta L-1 Con Paso 1 Haga
        reversa    <-reversa+ temporal[i-1]
        i<-i-1
    Fin Para
    devuelva reversa
Fin SubAlgoritmo
```



### Ejercicio 10

**Paso 1**: Definir el problema



**Paso 2**: Poner la entrada, proceso y salida

Entrada: lista

Proceso:

Se ordena alfabeticamente

- Se cuenta el numero de elementos de la lista y se asigna a n

- Se crea una variable listaOrdenada, que es donde se van a ordenar los nombres alfabeticamente

Salida: Escribir listaOrdenada

**Paso 3**: Escribir Pseudocódigo

``` Code Languaje
Algoritmo listaAlfabetica
	# Entrada
	lista <- leer
	# Proceso
	n<- contar el numero de elementos de la lista
	listaOrdenada <- lista
	j<-0
	Repetir 
		menorPalabra <- listaOrdenada[j]
		Para i = j Hasta n-1 con Paso 1 Hacer
			menor <- listaOrdenada[j]
			Si menorPalabra es mayor que listaOrdenada[i] Entonces
				menorPalabra <- listaOrdenada[i]
				posicion <- i
		FinPara
		Hasta que i sea igual a n
		temporal<-listaOrdenada[j]
		listaOrdenada[j]<-menorPalabra
		listaOrdenada[posicion]<-temporal
		k <- j+1
	
	Hasta Que j sea igual que n-2
	# Salida
	Escribir(listaOrdenada)
Fin Algoritmo
```



### Ejercicio 11

**Paso 1**: Definir el problema

¿Qué es un numero factorial? 

Si hay que calcular un el factorial de un numero, por ejemplo, 4, seria 1x2x3x4.

**Paso 2**: Poner la entrada, proceso y salida

Entrada: Asignamos un valor previamente validado a la variable `numero`

Proceso: 

- Bucle con la longitud del numero donde `factorial` será `factorial*(i+1)`

Salida: mostrar `factorial`

**Paso 3**: Escribir Pseudocódigo

``` Code Languaje
Algoritmo factorial
	# Entrada
	numero <- leer
	factorial <- 1
	# Proceso
	Para i=o en longitud numero con Paso 1 Hacer
		factorial <- factorial * (i+1)
	# Salida
	mostrar factorial
Fin Algoritmo
```



### Ejercicio 12

**Paso 1**: Definir el problema

¿Como saber si un numero es primo? Si es divisible solo entre 1 y si mismo

**Paso 2**: Poner la entrada, proceso y salida

Entrada: Asignamos un valor previamente validado a la variable `numero`

Proceso: 

- Comprobamos si el numero solo es divisible entre 1 y `numero`

Salida: mostrar comprobación

**Paso 3**: Escribir Pseudocódigo

``` Code Languaje
Algoritmo numeroPrimo
	# Entrada
	numero <- leer
	resultado <- 0
	primo <- true
	# Proceso
	Si numero es valido Entonces
		Para i=numero-1 Hasta 2 con Paso -1 Hacer
			resultado = numero mod i
			Si resultado = 0
				primo <- False
				i <- 2 #break
			FinSi
		FinPara
	FinSi
	# Salida
	Si primo es false Entonces
		Mostrar que no es primo
	Else
		Es primo
Fin Algoritmo
```



### Ejercicio 13

**Paso 1**: Definir el problema

Como calcular el area y volumen de un cubo dado su lado?

Volumen = lado x lado x lado

Area = 6 x lado al cuadrado 

**Paso 2**: Poner la entrada, proceso y salida

Entrada: Asignamos un valor previamente validado a la variable `lado`

Proceso: 

- Calculamos `volumen`,`area`

Salida: mostrar comprobación

**Paso 3**: Escribir Pseudocódigo

``` Code Languaje
Algoritmo areaYPerimetro
	# Entrada
	lado <- leer
	# Proceso
	Si lado es valido Entonces
		volumen <- lado * lado * lado
		area <- 6 *(lado*lado)
	Sino
		"Introduce numero válido"
	FinSi
	# Salida
	mostrar volumen
	mostrar area
Fin Algoritmo
```



### Ejercicio 14

**Paso 1**: Definir el problema

Coger de la lista introducida por el usuario y comprobar cual de ellos es par. Guardarlo en una variable que vaya aumentando conforme encuentra un numero par sumando este con el anterior

**Paso 2**: Poner la entrada, proceso y salida

Entrada: `listaNumeros` previamente validados

`par` inicializado a 0

**Paso 3**: Escribir Pseudocódigo

``` Code Languaje
Algoritmo listaNumerosEnterosPares
	# Entrada
	listaNumeros <- leer
	par <- 0
	# Proceso
	Si listaNumeros es valido Entonces
		Para i = 0 Hasta longitud listaNumeros con Paso 1 Hacer
			Si listaNumeros[i] mod 2 es igual a 0
				par <- par + listaNumeros[i]
		FinPara
	Sino
		"Introduce numeros correctos"
	FinSi
	# Salida
	mostrar par
Fin Algoritmo
```



### Ejercicio 15

**Paso 1**: Definir el problema

Definir si un numero es mayor, igual o menor que 0

**Paso 2**: Poner la entrada, proceso y salida

Entrada: `numero` que se valida posteriormente

Proceso: 

- Comprobar si es mayor, igual o menor que 0

Salida: Mostrar que caso es

**Paso 3**: Escribir Pseudocódigo

``` Code Languaje
Algoritmo mayorIgualMenor
	# Entrada
	numero <- leer
	mayor <- False
	menor <- False
	igual <- False
	# Proceso
	Si numero es valido Entonces
		Si numero es mayor a 0
			mayor <- True
		Sino numero es igual a 0
			igual <- True
		Sino numero es menor que 0
			menor <- True
		FinSi
	Sino
		"Introduce numero correcto"
	FinSi
	# Salida
	mostrar la variable que sea True
Fin Algoritmo
```



### Ejercicio 16

**Paso 1**: Definir el problema

Para calcular la media, se suman los números introducidos y se divide entre la cantidad de números que se han escrito

**Paso 2**: Poner la entrada, proceso y salida

Entrada: `listaNumeros` será la lista o array que almacene esos numeros.

Proceso: 

- Si son validos los numeros, los numeros se iran sumando uno a uno en un bucle y almacenando en una variable auxiliar `suma`. Después, `suma` se divide entre la longitud del array -1 porque el array empieza en 0 y se almacena en `media`

Salida: mostrar `media`

**Paso 3**: Escribir Pseudocódigo

``` Code Languaje
Algoritmo media
	# Entrada
	listaNumeros <- leer
	suma <- 0
	media <- 0
	# Proceso
	Si listaNumeros es valido Entonces
		Para i=0 Hasta longitud listaNumeros con Paso 1 Hacer
			suma <- suma + listaNumeros[i]
		FinPara
	Sino
		"Introduce numeros correctos"
	FinSi
	media <- suma / (longitud listaNumeros -1)
	# Salida
	mostrar media
Fin Algoritmo
```



### Ejercicio 17

**Paso 1**: Definir el problema

Comprobar si el numero introducido es mayor, igual o menor que el numero aleatorio

**Paso 2**: Poner la entrada, proceso y salida

Entrada: `numeroAleatorio` ,`numero` ,`valido` 

Proceso: 

- `numeroAleatorio` será un numero dado por el sistema

- `numero` será el numero que vaya introduciendo el usuario para adivinar

- `valido` será la variable inicializada en False para que no salga del bucle hasta que `numero` sea igual a `numeroAleatorio`

Salida:

mostrar Verdadero o falso

**Paso 3**: Escribir Pseudocódigo

``` Code Languaje
Algoritmo aleatorio
	# Entrada
	numeroAleatorio <- por el sistema
	numero <- leer
	valido <- False
	# Proceso
	Mientras sea valido hacer
		Si numero < numeroAleatorio Entonces
			Mostrar "Es menor"
			numero <- leer
		Sino numero > numeroAleatorio Entonces
			Mostrar "Es mayor"
			numero <- leer
		Sino
			valido <- true
		FinSi
	FinMientras
	# Salida
	Mostrar resultado "Correcto, tu numero es " + numero + " y el numero aleatorio era " + numeroAleatorio  
Fin Algoritmo
```



### Ejercicio 18

**Paso 1**: Definir el problema

Un anagrama es una palabra que está escrita con las mismas letras y es otra palabra diferente

**Paso 2**: Poner la entrada, proceso y salida

Entrada: `cadena1`, `cadena2`

Proceso: 

- Se cuenta el numero de elementos de `cadena1` y numero de elementos de `cadena2`, asignándose estos valores a n y m, respectivamente
- Si n y m son iguales:
  - Asignar a i el valor 0
  - Se asigna a `resultado` el valor es `anagrama`.
    - Mientras `i` sea menor o igual que `n-1:`
      - Se asigna a `noEstaLetra` el valor `True`.
      - Para `j` empezando en `i` hasta que sea igual que `n-1`:
        - Si `cadena1[i]` es igual a `cadena2[j]` entonces:
          - la posicion `j` en la que está `cadena[i]` se asigna a la posicion
          - Se asigna a `noEstaLetra` el valor `False`
        - Si `noEstaLetra` tiene valor `True`:
          - Se asigna a `resultado` el valor "no es anagrama"
          - Se asigna a `i` el valor `n`
        - Sino:
          - Se asigna a `temporal` el `elemento2[i]`
          - Se asigna a `cadena2[i]` igual a `cadena1[i]`
          - Se asigna `cadena[posicion]` igual a `temporal`
          - Se asigna a `i` el valor `i+1`

Salida: Escribir(`resultado`)

**Paso 3**: Escribir Pseudocódigo

``` Code Languaje
Algoritmo anagrama
	# Entrada
	cadena1 <- leer
	cadena2 <- leer
	# Proceso
	n <- contarElementosLista(cadena1)
	m <- contarElementosLista(cadena2)
	Si n es igual a m
		i <- 0
		resultado <- "Es anagrama"
		Mientras i sea menor o igual que n-1
			noEstaLetra <- True
			Para j=i Hasta n-1 con paso 1 Hacer
				Si cadena1[i] es igual a cadena2[j] Entonces
					posicion <- j
					noEstaLetra <- False
				FinSi
			FinPara
			Si noEstaLetra es igual a True Entonces
				resultado <- "no es anagrama"
				i <- n
			Sino
				temporal <-cadena2[i]
				cadena2[i] <- cadena1[i]
				cadena2[posicion] <- temporal
				i <- i+1
			FinSi
		FinMientras
	FinSi
	# Salida
	Mostrar resultado
Fin Algoritmo
```



### Ejercicio 19

**Paso 1**: Definir el problema

Comprobar que los números estén repetidos

**Paso 2**: Poner la entrada, proceso y salida

Entrada: `listaNumeros`, `arrayUnico`

Proceso:

- Validamos los números de `listaNumeros`
- Hacemos un bucle para comprobar si los numeros están en un array vacio llamado `arrayUnico`. Si está, significa que está repetido, por lo que no lo incluimos en `arrayUnico`
- Mostramos `arrayUnico`

Salida: mostrar `arrayUnico`

**Paso 3**: Escribir Pseudocódigo

``` Code Languaje
Algoritmo duplicados
	# Entrada
	listaNumeros <- leer
	arrayUnico <- []
	# Proceso
	Para i Hasta longitud listaNumeros con Paso 1 Hacer
		Si listaNumeros[i] no está en unico Entonces
        	añadir listaNumeros[i] a arrayUnico #con un append o parecido
		FinSi
	FinPara
	# Salida
	Mostrar arrayUnico
Fin Algoritmo
```



### Ejercicio 20

**Paso 1**: Definir el problema

Un numero es capicua cuando es igual leido de izq a der que de der a izq: Ej 1331

**Paso 2**: Poner la entrada, proceso y salida

Entrada: `numero`, `valido`, `arrayNum`

Proceso: 

- Se valida que `numero` sea de verdad un digito.

- `numero` se mete en un array `arrayNum`

- Comprobamos en un bucle la primera posición con la ultima y así sucesivamente. Si las posiciones que comparamos en cada vuelta son iguales, `valido` se mantiene en True, si no, será False y saldrá del bucle.

Salida: Si `valido` se mantiene en True, el numero es capicúa, si no, no lo es

**Paso 3**: Escribir Pseudocódigo

``` Code Languaje
Algoritmo capicua
	# Entrada
	numero <- leer
	valido <- True
	# Proceso
	Para i=0 Hasta longitud arrayNum con Paso 1 Hacer
		Si arrayNum[i] no es igual a arrayNum[-i-1] Entonces
			valido<- False
			exit
		FinSi
	FinPara
	# Salida
	mostrar valido
Fin Algoritmo
```



