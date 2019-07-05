#PROGRAMACIÓN BÁSICA 
## TUTORIAL DE PYTHON

##TEMA 1.CONCEPTOS BÁSICOS 
####¿Qué es Python?
>Es un lenguaje de programación, creado por Guido van Rossum a los principios de los años 90, cuyo nombre esta inspirado en el grupo de cómicos ingleses "Monty Python". Es un lenguaje similar a "C", pero con una sintaxis muy limpia y que favorece un código legible.

EJEMPLO :                                                     
    
    (Lenguaje "C"):                                                                                                                                                
    # include <stdio.h>                                             
    void.mainvoid{printf"Hola"}
    printf(" a tod@s")
    
    (Lenguaje Python):
    print('Hola a tod@s')
 
----
#### Lenguaje interpretado o de script
>Un lenguaje interpretado o de script es aquel que se ejecuta utilizando un programa intermedio llamado **intérprete**. En lugar de compilar el código a lenguaje máquina que pueda comprender y ejecutar directamente una computadora (lenguajes compilados). 
>La ventaja de lo lenguajes compilados es que su ejecución es mas rápida sin embargo los los lenguajes interpretados son mas flexibles y portados.

>**Interprete: Python, Java, Matla, Basic Ruby**

>**Compilado: HTML, Pascal**


----
##TEMA 2.INTRODUCCIÓN A LOS EJERCICIOS DE PROGRAMACIÓN 
Los ejercicios estan diseñados para volverse familiar la sintaxis de Python desarrollando los siguientes temas:

    1.Generar una salida con la sentencia print.
    2.Leer la entrada del usuario con el teclado usando "raw-input".
    3.Realizar cálculos sencillos como suma +, resta -, multiplicación *, división % y potencia **.
    4.Realizar cálculos más complejos con el módulo "math".

Para entrar a la terminal se debe escribir el comando **Python**. 

Para salir de **Python** debemos escribir **exit()**.

>Existen dos formas de ejecutar código Python, la cual puede ser mediante una sesión interactiva (línea a línea) con el intérprete, o bien de la forma habitual, escribiendo el código en un archivo de código fuente y ejecutándolo. En la primera parte de este tutorial lo haremos con el interprete.

El primer programa que vamos a escribir en Python es el clásico **"Hola Mundo"**, y en este lenguaje es tan simple como:
   
                  print ('Hola Mundo')
    Donde print: Es el comando 
    Donde 'Hola Mundo': Son el argumento o cadena de texto 

###Cadena de texto 
Ejemplo:
    
         mi_cadena='Tengo hambre y faltan 60 minutos para salir'
         print(mi_cadena)
         >>Un comentario en python inicia con el carácter reservado "#"
         Variable = mi_cadena
         Valor = 'Tengo hambre y faltan 60 minutos para salir'

###Tipos de datos básicos 
En python los tipos de datos básicos se dividen en:

>•	 Números, como pueden ser 3 (entero), 15.57 (de coma flotante) o 7 + 5j (complejos)

>•	 Cadenas de texto, como “Hola Mundo”

>•	 Valores booleanos: True (cierto) y False (falso).

Para poder conocer el tipo de dato de una variable usaremos la instruccion **type()**

Como se puede notar a diferencia de muchos otros lenguaje. en python no se puede declarar el tipo de variable al crearla.

En python se pueden representar numeros enteros, reales y complejos, donde los numero enteros se representan con la variable **(int)** la cual puede almacenar numero en la plataforma de 64 bits. 

Los numeros flotantes son los que tienen decimales. En python se expresa mediante el tipo **(float)**.

Los numeros complejos son aquellos que tienen una parte imaginaria. Para definir una variable compleja se utiliza en termino **Complex**.

Ejemplo:

    # esto es una cadena
    c = “Hola Mundo”
    # y esto es un entero
    e = 23
    # podemos comprobarlo con la función type
    type(c)
    type(e)
    
###Operadores 
>Veamos ahora qué podemos hacer con nuestros números usando los operadores por defecto. Para operaciones más complejas podemos recurrir al **módulo math.**

####Operadores aritméticos
    Operador   Descripción           Ejemplo
       +          Suma        r = 3 + 2 # r es 5
       -          Resta       r = 4 - 7 # r es -3
       -        Negación      r = -7 # r es -7
       *     Multiplicación   r = 2 * 6 # r es 12
       **       Exponente     r = 2 ** 6 # r es 64
       /        División      r = 3.5 / 2 # r es 1.75
      //     División entera  r = 3.5 // 2 # r es 1.0
       %         Módulo       r = 7 % 2 # r es 1

###Tipos de variables 

Es un nombre que se refiere a un objeto que reside en la memoria. El objeto puede ser de alguno de los tipos vistos (número o cadena de texto), o alguno de los otros tipos existentes en Python.

    String----> 'Blanca'=Cadena de texto 
    Integer----> 18 = Número 

###Concatenar 
>Unir varias variables del tipo **String** en una sola.

###Salto de linea 
>Para poder hacer un salto de linea tendro de un comando debemos agregar **'\n'**

Ejemplo:

    print(nombre + '\n' + calle)

###Variable "input()"
>Permite obtener texto escrito por teclado. Al llegar a la función, el programa se detiene esperando que se escriba algo y se pulse la tecla Intro, como muestra el siguiente ejemplo:

    print('Inserta tu nombre')
    nombre=input()
    print('Hola' + nombre)

###Variable flotante 
>Es una variable que puede guardar datos numéricos con punto decimal, para forzar a una variable a que sea flotante usaremos el comando **float()**.

    float=número decimal
    int=número entero

##TEMA 3.CONTROL DE FLUJO 
###Sentencias condicionales 
>Si un programa no fuera más que una lista de órdenes a ejecutar de forma secuencial, una por una, no tendría mucha utilidad. Los condicionales nos permiten comprobar condiciones y hacer que nuestro
programa se comporte de una forma u otra, que ejecute un fragmento de código u otro, dependiendo de esta condición.

>Aquí es donde cobran su importancia el tipo booleano y los operadores lógicos.

####Condicional if...else
La forma más simple de un estamento condicional es un if (del inglés SI) seguido de la condición a evaluar, dos puntos (:) y en la siguiente línea e indentado, el código a ejecutar en caso de que se cumpla dicha condición.
 
    LINEA 1  if comparación o condición:
    LINEA 2  identación(4espacios) #Código a ejecutar 
                                   en caso de que la 
                                   condición sea verdadera 
    LINEA 3  else: 
    LINEA 4  identación(4espacios) #Código a ejecutar 
                                   en caso de que la  
                                   condición sea falsa 

                              Comparación
                             a=b ---> a==b
                     a no es igual a  b ---> a!=b
                             a>b ---> a>b
                             a<b ---> a<b
                   a es mayor o igual a b ---> a>=b
                   a es menor o igual a b ---> a<=b

Ejemplo:

    entero=int(input('Introduzca un numero entero: '))
    par=entero%2
    if par == 0:
        print('El numero es par')
    else:
        print('El numero no es par')


![ejercicio17](https://user-images.githubusercontent.com/52331386/60689799-08fbbd00-9e87-11e9-9988-3a44cff4fee7.png)


####Sentencias if 
Nos encontraremos con  sentencias que tendrán que ver con el ámbito matemático ya sea graficar vectores o simplemente crear uno  de ellos , por lo que se usaran los siguientes códigos:

    import "numpy" as "np"
    import "matplotlib.pyplot" as "plt"

    #Creando un vector númerico 
       x = np.orange(100)
       y = np.sin(x)
    #Graficando
       plt.plot (x,y)
       plt.show ()

 
###Bucles 

>Mientras que los condicionales nos permiten ejecutar distintos fragmentos de código dependiendo de ciertas condiciones, los bucles nos permiten ejecutar un mismo fragmento de código un cierto número de veces, mientras se cumpla una determinada condición.

####While
El bucle while (mientras) ejecuta un fragmento de código mientras se cumpla una condición.Tiene la siguiente estructura:

    While condición:
    ____ fragmento_de_codigo_que_se_repita

Tenemos un comando que nos ayuda a romper el ciclo while y es: **Break**

Ejemplo:

    edad=0
    while edad < 19 :
        print('Tienes ', edad )
        edad=edad+1

    print ('fin de programa')

![ejercicio20-1](https://user-images.githubusercontent.com/52331386/60689948-95f34600-9e88-11e9-8153-03f84cb75d1e.png)

####Ciclo for....in

 En Python for se utiliza como una forma genérica de iterar sobre una sola secuencia, es decir, recorrer una secuencia.

Este es el aspecto de un bucle for en Python:

    secuencia = [“uno”, “dos”, “tres”]
    for elemento in secuencia:
        print (elemento)

Ejemplo:

    for celcius in range(0,101,10):
        farenheit = (1.8*celcius)+32
        print(celcius,'gC','|',farenheit,'gF')

![ejercicio21](https://user-images.githubusercontent.com/52331386/60690066-ea4af580-9e89-11e9-9b5a-aea183f5eded.png)


##TEMA 4. FUNCIONES 

>Una función es un fragmento de código con un nombre asociado que realiza una serie de tareas y devuelve un valor.

>Además de ayudarnos a programar y depurar dividiendo el programa en partes las funciones también permiten reutilizar código.

Las funciones ayudan al programador a dividir un problema en pequeñas piezas que pueden ser reusadas, tambien ayudan a concentrarse a una pequeña parte del programa a la vez. Como resultado el escribir funciones es una parte importante del desarrollo de sofware.

En Python las funciones se declaran de la siguiente forma:

    def mi_funcion(param1, param2):
        print param1
        print param2

Ejemplo:

    def areaTriangulo(base,altura):
        return (base*altura)/2.

    area=areaTriangulo(2.4,4.3)
    area1=areaTriangulo(5.4,3.2)
    area2=areaTriangulo(5.4,4.2)
    print(area,'\n',area1,'\n',area2)

![ejercicio24](https://user-images.githubusercontent.com/52331386/60690268-b7a1fc80-9e8b-11e9-8526-ca05475a1ec3.png)


##TEMA 5.GRÁFICOS
Hay muchos módulos en python que proveen características poderosas que podemos usar en nuestros propios programas. Algunos de estos pueden enviar correos electrónicos y algunos pueden extraer información de paginas d Internet. Para el manejo de gráficos usaremos un modulo que perite crear figuras y patrones. El modulo que se usara permite desarrollar nuestro pensamiento computacional.
 
>El modulo se llama: **Turtle**

Ejemplo:

    import turtle
    ventana=turtle.Screen()
    alex=turtle.Turtle()
    alex.forward(100)
    alex.left(90)
    alex.forward(100)
    alex.left(90)
    alex.forward(100)
    alex.left(90)
    alex.forward(100)
    alex.left(90)
    alex.forward(100)
    ventana.mainloop()

![ejercicio27](https://user-images.githubusercontent.com/52331386/60690664-b1f9e600-9e8e-11e9-97f9-052290474764.png)

##TEMA 6. PROGRAMACIÓN ORIENTADA A OBJETOS
> Es un paradigma de programación en el que los conceptos del mundo real relevantes para nuestro problema se modelan a través de clases y objetos, y en el que nuestro programa consiste en una serie de interacciones entre estos objetos.

###Clases y objetos 
####¿Qué es un objeto?

>Un objeto es una entidad que agrupa un
estado y una funcionalidad relacionadas. El estado del objeto se define a través de variables llamadas atributos, mientras que la funcionalidad se modela a través de funciones a las que se les conoce con el nombre de métodos del objeto.

Un ejemplo de objeto podría ser un coche, en el que tendríamos atributos como la marca, el número de puertas o el tipo de carburante y métodos como arrancar y parar. O bien cualquier otra combinación de atributos y métodos según lo que fuera relevante para nuestro programa.

####¿Qué es una clase?

>Una clase, por otro lado, no es más que una plantilla genérica a partir de la cuál instanciar los objetos; plantilla que es la que define qué atributos y métodos tendrán los objetos de esa clase.

En Python las clases se definen mediante la palabra clave class seguida del nombre de la clase, dos puntos (:) y a continuación, indentado, el cuerpo de la clase. Como en el caso de las funciones, si la primera línea del cuerpo se trata de una cadena de texto, esta será la cadena de documentación de la clase o docstring.

Ejemplo:
    
    class Coche(object):
        def __init__(self,gasolina):
            self.gasolina = gasolina
        def arrancar(self):
            if self.gasolina > 0:
                print('Arranca')
            else:
                print('No Arranca')
        def conducir(self):
            if self.gasolina > 0:
                self.gasolina = self.gasolina - 1
                print('Quedan ', self.gasolina,' litros')
            else:
                print('No se mueve')
    vocho = Coche(5)
    tsuru = Coche(3)

    vocho.arrancar()
    vocho.conducir()
    vocho.conducir()
    vocho.conducir()
    vocho.conducir()
    vocho.conducir()
    vocho.conducir()

![ejercicio35](https://user-images.githubusercontent.com/52331386/60690922-0d2cd800-9e91-11e9-946c-f9181d3d2cef.png)

##7. EJERCICIOS REALIZADOS EN CLASE 

####TEMA 2.INTRODUCCIÓN A LOS EJERCICIOS DE PROGRAMACIÓN
----
Ejercicio 1.

    nombre='Marco Ivan'
    calle='Francisco J. Mujica #119'
    colonia='Constituyentes de 1917'
    municipio='Huixquilucan'
    estado='Estado de Mexico'
    codigo=52775

    print(nombre + '\n' + calle + '\n' + colonia + '\n' + municipio + '\n' + estado + '\n' , codigo)


![ejercicio1](https://user-images.githubusercontent.com/52331386/60691338-9db8e780-9e94-11e9-8705-6c1ce5bc4f1b.png)

Ejercicio 2. 

    print('ingresa tu nombre')
    nombre=input()
    print('hola ' + nombre)

Ejercicio 3.
   
    l=float(input('Ingresa el largo de la habitación 
    en metros: '))
    a=float(input('Ingrese el ancho de la habitación 
    en metros: '))
    R= l*a

    print('El area de la habitacion es:' , R , 
    'metros cuadrados')  

![ejercicio3](https://user-images.githubusercontent.com/52331386/60691704-3e100b80-9e97-11e9-9fc2-06dacbd5b55a.png)

Ejercicio 4.

    largo=float(input('Cual es el largo de una cancha de fubol? '))
    ancho=float(input('Cual es el ancho de una chancha de futbol? '))
    area_metros=largo*ancho
    area=float(area_metros*0.000247105)

    print('El area de la cancha de futbol es de', area, 'en acres')

![ejercicio4](https://user-images.githubusercontent.com/52331386/60691766-a0690c00-9e97-11e9-8e9c-7ad2d2ab23e0.png)

Ejercicio 5.

    print('Recicle Botellas')
    un_litro=int(input('Cuantas botellas vas a poner '))
    mas_litro=int(input('Cuantas botellas vas a poner de mas litros '))

    pago=(un_litro*mas_litro)
    pagom=(un_litro*1)
    pagon=float=(mas_litro*2.50)

    pagot=(pagom+pagon)

    print('se te va a dar $',pagot,'pesos')

![ejercicio5](https://user-images.githubusercontent.com/52331386/60691815-081f5700-9e98-11e9-95ae-b3e18850a281.png)

Ejercicio 6.

    print('Biembenido al restaurante Juanito')
    print('Carretera Naucalpan Toluca #794 Col. San 
    Rafael Chamapa  CP. 53660')
    print('Tu orden fue de: ')

    comida=input()
    costo=50
    print('Tu ',comida, 'vale $' ,costo)

    iva=0.16
    con_iva=float(costo*iva)
    print('Con IVA es $ ',con_iva)

    prop=0.10
    con_prop=float(costo*prop)
    print('Con propina son $' ,con_prop)

    total=con_iva+con_prop
    tot=costo+total
    print('Tu total es de $' ,tot)

![ejercicio6](https://user-images.githubusercontent.com/52331386/60691880-782ddd00-9e98-11e9-81be-931f323ec2bb.png)

Ejercicio 7.

    n=int(input('numero :'))
    s=int((n*(n+1))/2)
    print('El resultado es ', s)

![ejercicio7](https://user-images.githubusercontent.com/52331386/60691928-b4613d80-9e98-11e9-8e20-5f3fd247bbc3.png)

Ejercicio 8.

    w=int(input('Indique el numero de widget :'))
    g=int(input('Indique el numero de gizmos :'))
    p1=w*75
    p2=g*112
    pt=int(p1+p2)
    print('El peso total de los productos adquiridos es de ', pt , 'gramos')

![ejercicio8](https://user-images.githubusercontent.com/52331386/60691976-eecada80-9e98-11e9-94c5-149991929e1a.png)

Ejercicio 9.

    s=float(input('Indique la cantidad de saldo que tiene la cuenta :'))
    s1=float(s*0.4)+s
    s2=float((s*0.4)*2)+s
    s3=float((s*0.4)*3)+s
    print(' El saldo que se tendra en la primer aunalidad es de ', s1 , 'pesos','\n',
    'El saldo que se tendra en la segunda aunalidad es de ', s2, 'pesos','\n',
    'El saldo que se tendra en la tercera aunalidad es de ', s3, 'pesos')

![ejercicio9](https://user-images.githubusercontent.com/52331386/60692041-6436ab00-9e99-11e9-8f01-e6848cef0ffe.png)

Ejercicio 10.

    a=int(input('Incerta un numero '))
    b=int(input('Incerta otro numero '))

    s=a+b
    print('La suma es ' ,s)

    r=b-a
    print('La resta es ' ,r)

    m=a*b
    print('El producto es ' ,m)

    d=a/b
    print('El residuo es ' ,d)

    dd=b/a
    print('El resultado es ' ,dd)

    p=a**b
    print('El resultado de "a" a la "b" es ' ,p)

    import math 
    print('El logaritmo es ' ,math.log10(a))

![ejercicio10](https://user-images.githubusercontent.com/52331386/60692100-b4ae0880-9e99-11e9-9b40-66a4bdebcc70.png)

Ejercicio 11.

    g=int(input('Cuantos galones tiene? '))
    l=float(235.21/g)

    print('Usted tiene' ,l , 'en L/100Km')

    #1cm^3 es igual a 1mL y un litro tiene 1000mL por lo tanto hay 1000cm^3

![ejercicio11](https://user-images.githubusercontent.com/52331386/60692135-0060b200-9e9a-11e9-9a30-762516268226.png)

Ejercicio 12.

    import math
    t1=int(input('Indique la latitud del primer punto de la tierra en grados: '))
    g1=int(input('Indique la longitud del primer punto de la tierra en grados: '))
    t2=int(input('Indique la latitud del segundo punto de la tierra en grados: '))
    g2=int(input('Indique la longitud del segundo punto de la tierra en grados: '))

    st1=(math.sin(t1))
    st2=(math.sin(t2))
    ct1=(math.cos(t1))
    ct2=(math.cos(t2))
    cg12=(math.cos(g1-g2))

    ac=(math.acos(st1*st2+ct1*ct2*cg12))

    d=float(6371.01*ac)

    print('La distancia entre los puntos que siguen la superficie de la tierra es de', d)

![ejercicio12](https://user-images.githubusercontent.com/52331386/60692211-81b84480-9e9a-11e9-90be-63f3ba158e02.png)

Ejercicio 13.

    import math
    r=float(input('Indique el radio de un circulo :'))
    p=math.pi

    a=p*(r**2)

    v=((4/3)*p*(r**3))

    print('El area de un circulo es '," 
    {:.2f}".format(a),'\n', 'El volumen de una esfera es ',"{:.2f}".format(v))

![ejercicio13](https://user-images.githubusercontent.com/52331386/60692274-d065de80-9e9a-11e9-9548-541bca93b59d.png)

Ejercicio 14.

    #ESCRIBA UN PREOGRAMA QUE LE DIGA AL USUARIO EL 
    NUMERO DE DIAS, HORAS, MINUTOS Y SEGUNDOS, EL 
    PREOGRAMA DEBE CALCULAR Y DESPLEGAR EL NUMERO DE 
    SEGINDOS TOTALES

    print('Llene los siguientes datos.')
    d=float(input('Cuantos dias '))
    h=float(input('Cuantas horas '))
    m=float(input('Cuantos minutos '))
    s=float(input('Cuantos segundos '))
    t=s+(m*60)+(h*3600)+(d*86400)

    print('El tiempo en segundos es',t)

![ejercicio14](https://user-images.githubusercontent.com/52331386/60692334-220e6900-9e9b-11e9-91df-651606210d8a.png)

Ejercicio 15.

    from time import asctime
    print(asctime())

![ejercicio15](https://user-images.githubusercontent.com/52331386/60692387-6c8fe580-9e9b-11e9-9157-a5b70edd8350.png)

###TEMA 3.CONTROL DE FLUJO  
Ejercicio 16.

    humanos=float(input('Indique su edad humanos :'))
    perros1=((humanos-2)*(4))+21
    perros2=humanos*10.5
    if humanos > 2:
        print('la conversion de edad humanos a perros es de ',perros1)
    elif humanos < 0:
        print('favor de ingresar los datos de forma correcta')
    else: 
        print('la conversion de edad humanos a perros es de ',perros2)

![ejercicio18](https://user-images.githubusercontent.com/52331386/60692758-423f2780-9e9d-11e9-81df-538989ba8ac0.png)

Ejercicio 17.

    casilla=str(input('escoje una casilla? :'))

    if casilla == ('a1'):
        print('casilla negra')

    elif casilla == ('a3'):
        print('casilla negra')

    elif casilla == ('a5'):
        print('casilla negra')

    elif casilla == ('a7'):
        print('casilla negra')

    elif casilla == ('b2'):
        print('casilla negra')

    elif casilla == ('b4'):
        print('casilla negra')
 
    elif casilla == ('b6'):
        print('casilla negra')

    elif casilla == ('b8'):
        print('casilla negra')

    elif casilla == ('c1'):
        print('casilla negra')

    elif casilla == ('c3'):
        print('casilla negra')

    elif casilla == ('c5'):
        print('casilla negra')

    elif casilla == ('c7'):
        print('casilla negra')

    elif casilla == ('d2'):
        print('casilla negra')

    elif casilla == ('d4'):
        print('casilla negra')

    elif casilla == ('d6'):
        print('casilla negra')

    elif casilla == ('d8'):
        print('casilla negra')

    elif casilla == ('e1'):
        print('casilla negra')
 
    elif casilla == ('e3'):
        print('casilla negra')

    elif casilla == ('e5'):
        print('casilla negra')

    elif casilla == ('e7'):
        print('casilla negra')

    elif casilla == ('f2'):
        print('casilla negra')

    elif casilla == ('f4'):
        print('casilla negra')

    elif casilla == ('f6'):
        print('casilla negra')

    elif casilla == ('f8'):
        print('casilla negra')

    elif casilla == ('g1'):
        print('casilla negra')

    elif casilla == ('g3'):
        print('casilla negra')

    elif casilla == ('g5'):
        print('casilla negra')

    elif casilla == ('g7'):
        print('casilla negra')
 
    elif casilla == ('h2'):
        print('casilla negra')
 
    elif casilla == ('h4'):
        print('casilla negra')

    elif casilla == ('h6'):
        print('casilla negra')

    elif casilla == ('h8'):
        print('casilla negra')


    else:
        print('casilla blanca')

![ejercicio19](https://user-images.githubusercontent.com/52331386/60693010-34d66d00-9e9e-11e9-8781-260e1f21913b.png)

Ejercicio 18.

    llave='0123'
    pasword=''

    while pasword !=llave:
        print('pasword incorrecto')
        pasword=input('inserte su pasword:')
    

    print('felicidades, entraste al sistema')

![ejercicio20-2](https://user-images.githubusercontent.com/52331386/60693154-c04ffe00-9e9e-11e9-9737-f5496bcbf658.png)

Ejercicio 19.

    llave='0123'
    pasword=''
    while True :
        pasword=input('inserte su pasword:')
        if pasword== llave:
            print('felicidades, entraste al sistema')
            break
        else:
            print('pasword incorrecto')
            print('intente de nuevo')    


    print('fin de programa')

![ejercicio20-3](https://user-images.githubusercontent.com/52331386/60693232-29377600-9e9f-11e9-8192-8db02727917f.png)

Ejercicio 20. 

    for precio in range(4,201,5):
    precio=(precio+0.95)
    descuento = (precio*0.60)
    preciof=(precio-descuento)
    print(precio,'$','|',"{:.2f}".format(descuento),'|',"{:.2f}".format(preciof,'$'))

![ejercicio22](https://user-images.githubusercontent.com/52331386/60693328-803d4b00-9e9f-11e9-860a-35c964cc1c33.png)

Ejercicio 21.

    print(' ',1,2,3,4,5,6,7,8,9,10)
    for a in range(1,11,1):
        x=a*1
        b=a*2
        c=a*3
        d=a*4
        e=a*5
        f=a*6
        g=a*7
        h=a*8
        i=a*9
        j=a*10
        print(x,a,b,c,d,e,f,g,h,i,j)

![ejercicio23](https://user-images.githubusercontent.com/52331386/60693428-df02c480-9e9f-11e9-8dc2-f9e691951395.png)

###TEMA 4. FUNCIONES

Ejercicio 22.

    def tarifa(k):
        tarifa = 7.25+(7*k)
        if tarifa < 40:
            tarifa=40
        return tarifa
    

    k=float(input('Cuantos kilometros vas a recorrer'))
    b=tarifa(k)
    print (b)

![ejercicio25](https://user-images.githubusercontent.com/52331386/60693603-87b12400-9ea0-11e9-8338-84ce3db81a6c.png)

Ejercicio 23.

    def producto(envio):
        producto = 150+45*(envio-1)
        if envio==1:
            return 150
        elif envio==0:
            return 0
        return producto

    envio=float(input('Cuantos articulos vas a pedir? '))
    b=producto(envio)
    print (b)

![ejercicio26](https://user-images.githubusercontent.com/52331386/60693690-e1195300-9ea0-11e9-9c46-caad4ee719b7.png)

###TEMA 5.GRAFICOS 

Ejercicio 24.

    import turtle
    ventana=turtle.Screen()
    ventana.bgcolor("yellow")
    ventana.title("Hola, Kary bebe")
    kary=turtle.Turtle()
    kary.color("blue")
    kary.pensize(5)
    kary.forward(100)
    kary.left(120)
    kary.forward(100)
    ventana.mainloop()

![ejercicio28](https://user-images.githubusercontent.com/52331386/60693871-8502fe80-9ea1-11e9-9b31-f13fe60ae39d.png)

Ejercicio 25.

    import turtle
    ventana=turtle.Screen()
    ventana.bgcolor("black")
    ventana.title("Hola, Kary bebe")

    omar=turtle.Turtle()
    kary=turtle.Turtle()

    omar.shape("turtle")
    omar.color("green")
    omar.pensize(2)

    kary.shape("turtle")
    kary.color("red")
    kary.pensize(2)

    omar.speed(9)
    kary.speed(10)

    omar.penup()
    kary.penup()
    omar.setpos(0,-50)
    omar.pendown()
    omar.circle(50)
    kary.setpos(0,-100)
    kary.pendown()
    kary.circle(100)

    ventana.mainloop()

![ejercicio31](https://user-images.githubusercontent.com/52331386/60694087-808b1580-9ea2-11e9-951a-520979a58ae5.png)

Ejercicio 26.

    import turtle
    a=int(input('Introdizca el numero de circulos que 
    desea:'))

    ventana = turtle.Screen ()
    ventana.bgcolor("black")
    ventana.title("Hola Kary bebe")

    kary = turtle.Turtle()
    kary.shape("turtle")
    kary.color ("green")
    kary.pensize (2)

    kary.speed(8)

    for i in range(a):
  
        kary.penup()
        kary.setpos(0,-(i*10))
        kary.pendown()
        kary.circle(i*10)
  
    ventana.mainloop()

![ejercicio32](https://user-images.githubusercontent.com/52331386/60694213-ff804e00-9ea2-11e9-882f-001ae1d58adc.png)

Ejercicio 27.

    import turtle
    ventana=turtle.Screen()
    ventana.setup(1000, 500)
    ventana.tracer(0)
    ventana.addshape("mario.gif")

    mario=turtle.Turtle()
    mario.speed(0)
    mario.shape("mario.gif")

    mario.penup()
    mario.goto(-500, 0)

    while True:
        ventana.update()
        mario.forward(.5)

![ejercicio33](https://user-images.githubusercontent.com/52331386/60694318-5be36d80-9ea3-11e9-9915-caf6e5839c85.png)

Ejercicio 28.

    import turtle

    window= turtle.Screen()
    window.addshape("mario.gif")
    border= turtle.Turtle()

    border.speed(0)
    border.up()
    border.hideturtle()
    border.pensize(0)
    border.color('white')
    border.goto(500,500)
    border.down()
    border.goto(500,-500)
    border.goto(-500,-500)
    border.goto(-500,500)
    border.goto(500,500)


    camino=turtle.Turtle()
    camino.speed(0)
    camino.shape("mario.gif")

    camino.up()
    dx=1

    while True:
        x,y= camino.position()
        if x+dx>=500 or x+dx<=-500:
            dx=-dx
   
        camino.goto(x+dx,y)


    window.mainloop()

![ejercicio34](https://user-images.githubusercontent.com/52331386/60694519-0360a000-9ea4-11e9-90f1-a6303bcdc4d2.png)

Ejercicio 29.

    import turtle

    ventana=turtle.Screen()
    ventana.bgcolor('green')
    ventana.title('Funciones')

    omar = turtle.Turtle()
    d = 50
    omar.forward(d)
    omar.left(90)
    omar.forward(d)
    omar.left(90)
    omar.forward(d)
    omar.left(90)
    omar.forward(d)
    omar.left(90)

ventana.mainloop()

![ejercicio39](https://user-images.githubusercontent.com/52331386/60694925-82a2a380-9ea5-11e9-812e-d048ce8e892d.png)

Ejercicio 30.

    import turtle

    ventana=turtle.Screen()
    ventana.bgcolor('green')
    ventana.title('Funciones')

    omar = turtle.Turtle()
    d = 50

    for i in range(4):
        omar.forward(d)
        omar.left(90)

    ventana.mainloop()

![ejercicio40](https://user-images.githubusercontent.com/52331386/60695018-d6ad8800-9ea5-11e9-8c9b-152b7cd70208.png)


###TEMA 6.PROGRAMACIÓN ORIENTADA A OBJETOS
Ejercicio 31.

    class Triangulo(object):
        def __init__(self,angulo1,angulo2,angulo3):
            self.angulo1 = angulo1
            self.angulo2 = angulo2
            self.angulo3 = angulo3

        def ChecarAngulo(self):

            if self.angulo1+self.angulo2+self.angulo3 == 180:
                print('Es un triangulo')

            else:
                print('No es un triangulo')

    miTriangulo=Triangulo(90,30,60)

    miTriangulo.ChecarAngulo()

![ejercicio36](https://user-images.githubusercontent.com/52331386/60694745-cba62800-9ea4-11e9-8dc2-ea29021e92fe.png)

Ejercicio 32.

    class Cancion(object):
        def __init__(self,letra):
            self.letra = letra
    
        def cantame(self):
            print(self.letra)

    micumpleanos=Cancion(["...que cantaba el rey David," " hoy por ser dia de tu santo," " te las cantamos a ti."])

    micumpleanos.cantame()

![ejercicio38](https://user-images.githubusercontent.com/52331386/60694830-2049a300-9ea5-11e9-9ccb-b3c3eb39e566.png)

Ejercicio 33.

    import turtle

    def dibujar_cuadro(tur, d):

        for i in range(4):
            tur.forward(d)
            tur.left(90)

    ventana=turtle.Screen()
    ventana.bgcolor('green')
    ventana.title('Funciones')

    omar = turtle.Turtle()
    kary = turtle.Turtle()
    dibujar_cuadro(omar, 50)
    dibujar_cuadro(kary, 200)

    ventana.mainloop()

![ejercicio41](https://user-images.githubusercontent.com/52331386/60695111-33a93e00-9ea6-11e9-9627-97f780a842e4.png)

Ejercicio 34.

    import turtle

    def dibujar_cuadro(tur, d):

        for i in ['red','purple','blue','yellow']:
            tur.color(i)
            tur.forward(d)
            tur.left(90)

    ventana=turtle.Screen()
    ventana.bgcolor('green')
    ventana.title('Funciones')

    omar = turtle.Turtle()
    kary = turtle.Turtle()
    dibujar_cuadro(omar, 50)
    dibujar_cuadro(kary, 200)

    ventana.mainloop()

![ejercicio42](https://user-images.githubusercontent.com/52331386/60695191-7d922400-9ea6-11e9-9479-1e851fa8cd95.png)

Ejercicio 35.

    import turtle

    def dibujar_multiples_cuadro(tur, d):

        for i in ['red','purple','blue','yellow']:
            tur.color(i)
            tur.forward(d)
            tur.left(90)

    ventana=turtle.Screen()
    ventana.bgcolor('black')
    ventana.title('Funciones')

    omar = turtle.Turtle()
    omar.pensize(3)

    d=20
    for i in range(50):
        dibujar_multiples_cuadro(omar, d)
        d = d+10
        omar.forward(10)
        omar.right(18)

    ventana.mainloop()

![ejercicio43](https://user-images.githubusercontent.com/52331386/60695315-eed1d700-9ea6-11e9-8326-7696dc04d461.png)

Ejercicio 36.

    import turtle


    def dibujar_cuadro_seguir(tur, p):
        for i in range(4):
            tur.forward(20)
            tur.left(90)
    

    ventana=turtle.Screen()
    ventana.bgcolor('blue')
    ventana.title('funciones')

    omar=turtle.Turtle()
    omar.pensize(5)
    omar.speed(2)

    p=30

    for i in range(5):
        dibujar_cuadro_seguir(omar, 5)

        omar.penup()
        omar.setpos(p,0)
        omar.pendown()
        p=p+30

![ejercicio44](https://user-images.githubusercontent.com/52331386/60695427-4a9c6000-9ea7-11e9-9f14-9c59f7ffbdb9.png)

Ejercicio 37.

    import turtle

    def dibujar (tur,d):
        for i in range(4):
            tur.color('blue')
            tur.forward(d)
            tur.left(90)
     
     
    ventana=turtle.Screen()
    ventana.bgcolor('black')
    ventana.title('funciones')

    alex=turtle.Turtle()
    alex.pensize(3)
    alex.speed(20)

    m=-10

    for i in range(20,1591,20):
        dibujar(alex,i)
        alex.penup()
        alex.goto(m,m)
        alex.pendown()
        m=m-10

    ventana.mainloop()


![ejercicio45](https://user-images.githubusercontent.com/52331386/60695523-95b67300-9ea7-11e9-8103-c7077b2d1267.png)

Ejercicio 38.

    import turtle

    def dibujar_cuadro(tur, d):
    
        for i in range(8):
            tur.forward(d)
            tur.left(45)
        
    ventana=turtle.Screen()
    ventana.bgcolor('white')
    ventana.title('funciones')

    a=turtle.Turtle()
    dibujar_cuadro(a, 50)

    ventana.mainloop()

![ejercicio46](https://user-images.githubusercontent.com/52331386/60695590-e037ef80-9ea7-11e9-9190-ef1800c2f315.png)

Ejercicio 39.

    import turtle

    def dibujar_cuadro_caracol(tur, d):
        for i in  ['red','blue','green','yellow']:
            tur.color(i)
            tur.forward(d)
            tur.left(90)

    ventana=turtle.Screen()
    ventana.bgcolor('black')
    ventana.title('funciones')

    alex=turtle.Turtle()
    alex.pensize(2)
    alex.speed(100)

    d=100

    for i in range(20):
        dibujar_cuadro_caracol(alex, d)
    
        alex.forward(10)
        alex.right(18)
        alex.setpos(0, 0)


    ventana.mainloop()

![ejercicio47](https://user-images.githubusercontent.com/52331386/60695662-28efa880-9ea8-11e9-9a63-6e463c38cbe9.png)

Ejercicio 40.

    import turtle

    def cuadrado(tur, d):
        for i in  range(200):   
            tur.forward(d)
            tur.left(90)
            d=d+5
        
    ventana=turtle.Screen()
    ventana.bgcolor('blue')
    ventana.title('funciones')


    d=15
    alex=turtle.Turtle()
    alex.speed(10)

    cuadrado(alex, d)

    ventana.mainloop()

![ejercicio48](https://user-images.githubusercontent.com/52331386/60695731-69e7bd00-9ea8-11e9-9a95-1fc06c302428.png)

Ejercicio 41.

    import turtle

    def cuadrado(tur, d):
        f=90
        for i in  range(500):
            tur.color('blue') 
            tur.forward(d)
            tur.left(f)
            d=d+5
            f=f+0.02
        
    ventana=turtle.Screen()
    ventana.bgcolor('black')
    ventana.title('funciones')

    d=15
    alex=turtle.Turtle()
    alex.speed(25)

    cuadrado(alex, d)

    ventana.mainloop()

![ejercicio49](https://user-images.githubusercontent.com/52331386/60695802-b3d0a300-9ea8-11e9-8bce-a1bcc4460129.png)


----
* Felipe Hernández Blanca Cecilia 
* Grupo B1
* Profesor. Enrique Garcia Trinidad 
* Programación Básica 
* 04-Jul-2019
* Ingeniería Mecatronica
