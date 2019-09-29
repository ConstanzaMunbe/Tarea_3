## Tarea_3

# Desarrollo Guía

1 - 
listaDeNumeros[0]
listaDeNumeros[15]
listaDeNumeros[-2]

- 0:Arrojó "list()".
- 15(mayor al largo de la lista):Arrojó "NULL", no existe la posición que se pidió.
- -2(numero negativo en el largo de elementos de la lista):Arroja todos los elementos de
 la lista, excepto el numero que corresponde a la posición 2.

2 - 
unlist(listaDeNumeros[2])

if(listaDeNumeros[5]+1>0){
  print("se cumple")
}

if(unlist(listaDeNumeros[5])+1>0){
  print("se cumple")
}

Al ejecutar el if con el unlist, se puede realizar la operación pedida, porque unlist
entrega solo el valor que corresponde a la posición que se pide, si se ejecuta con la 
variable que corresponde a la lista


3 -
listaDeNumeros[5] <- 12

Lo que ocurre al ejecutar "listaDeNumeros[5]" solo se imprime lo mismo en la consola, 
estableciendo el nuevo valor asignado para dicha variable.


4 -
length(listaDeNumeros)

Al ejecutar length(listaDeNumeros) arroja la cantidad de elementos que contiene 
la lista.

5 -
valorInicial : valorFinal

valorInicial <- 5
  valorFinal <- 11
  

valorInicial <- 11
  valorFinal <- 5  
  
Dejando de valor incial 5 y final 11, se muesta la lista con los elementos de 5 
al 11 en orden ascendente, luego al invertir los valores, se mestran los valores
en orden descendente.


  length(listaDeNumeros) : valorFinal
  
Al ejecutar el length de listaDeNumeros : valor inicial <- 11, se establece el largo 
de la lista (11) y el valor final con valor 11, parte y termina en el mismo número,
pero si se establece el valor vinal 5, se da el espacio para que el length recorra
desde la cantidad de elementos en total (11) y hasta el valor 5, los recorre
y ordena descendentemente.


6 -
for(i in 1 : 100){
    print(paste("cuento ",i," flores"))
  }

Al ejecutar el for, ocurre una iteración de i desde el 1 al 100, dando por cada uno
de los valores un resultado ed un print "cuento "i" flores, para obtener el conteo 
completo del rando 1 : 100

7 -
for(i in listaDeNumeros){
    print(listaDeNumeros)
  }

Se reemplazó la iteración numérica por la iteración de la listaDeNumeros
y al ejecutar se imprimió la posicón de la lista con el valor que le corresponde,
sin ordenar secuencialmente.


8 -
for(i in listaDeNumeros){
   if(i%%2 ==0){
    print("par")
  }else{
      print("impar")
    }
 
}
 

Ocupé la función for para hacer una iteración numérica dentro de la lista listaDeNumeros,
para ocupar un if que condicione la iteración mediante una división de 2, para 
que este entregue un resultado en decimal, los numeros que entreguen un resultado
 decimal ==0, se imprimirá "par" y los que sean !=0 imprimirá"impar", estos últimos
son captados con la funcion else. 

9 - (respuesta incompleta)
Para generar una lista de 100 resultados aleatorios entre Si y No, hice
un sample de 0:100.
Asigné a la lista como un objeto para ser procesada con el comando for.

Se intentó hacer un loop con la lista mencionada para obtener datos aleatorios de
100 votantes.
FALTA: PROCESAR LA LISTA CON LAS REGLAS DEL QUÓRUM Y HALLAR LOS POSIBLES CANDIDATOS QUE
VOTEN SI O NO Y HALLAR EL PORCETAJE DE CADA OPCIÓN.

*intento de respuesta*


listaDeVotos <- sample(0:1, 100, replace=T)

for( votante in listaDeVotos){
  if(votante == 1){
    print("Si")
      }else{
        print("No")
      }
   
}


10- 

Suma <- function(a,b){
  a+b
}

Resta <- function(a,b){
  a-b
}

Division <- function(a,b){
  a/b
}

Multiplicacion <- function(a,b){
  a*b
}


Suma(3,5)
Resta(6,3)
Division(12,3)
Multiplicacion(2,5)

A cada operación matemática, se le asignó una función que procesa los 
parametros (a,b), para que al introducir números en los parametros éstos sean
procesados en la función. Si se agrega un valor extra en la operación, que no esté 
determinado en el function, este no será procesado y será un argumento no utilizado, 
esto causará que la operación matemática que queremos realizar no se pueda ejecutar.

11 -
areaRectangulo <- function(a1,b1,a2,b2){
  (a1*b1) - (a2*b2)
}
areaRectangulo(2,4, 2,3)

Se creó una función (areaRectangulo) que procesará 4 datos entregados que
posteriormente se procesaran para realizar una diferencia de las areas de 2 rectangulos
obteniendo así el resultado deseado. *(a1*b1 sera el area del rectangulo mas grande)*

pi <- 3.1415

areaCirculo <- function(r1,r2){
  pi*(r1^2) - pi*(r2^2)
}
areaCirculo(6,4)


Con la misma lógica la funcion (areaRectangulo), se modificó para que opere con los datos necesarios
para calcular el área de los círculos, éste requirió establecer el valor de pi.


**opcional** -
for( i in listaDeNumeros){
  print(i)
}

La ventaja es que se pueden ver los elementos de la lista en el orden establecido en ella, 
la desventaja es que no se especifica a que posición de la lista corresponde cada valor, 
ya que antes de cada valor aparece [1] y no la ubicación de los valores dentro la lista.