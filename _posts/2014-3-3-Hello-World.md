---
layout: post
title: TESTING jekyll-now
---

El hashing ó _Message Digest_ es una función matematica a la cual le damos un **INPUT**, y nos devuelve un **OUTPUT** fijo del mismo tamaño y unico para ese **INPUT** en especifico. Ese **INPUT** pudiera ser una imagen, un audio, una contraseña o cualquier tipo de archivo que tengamos.  

Digamos que tenemos la contraseña **123Abc**, y tenemos la contraseña **123abc**  

MD5 123Abc -> **876dfefef3ef6f4548f48bbddd856cef**  
MD5 123abc -> **a906449d5769fa7361d7ecc6aa3f6d28**  

Lo que significa que la funciones de hashing son case-sensitive, cuaquier cambio de mayusculas a minusculas cuenta, cualquier cambio en uno de los caracteres cuenta.

En el caso de MD5, nos devuelve un largo fijo de 128 bits, pero sí contamos la cantidad de caracteres nos fijamos que tenemos 32.  
32 x 4 = 128 bits. El **OUTPUT** de MD5 no es un "STRING" sino mas bien caracteres hexadecimales, cada caracter hexadecimal (0-9)(A-F) es representado en la computadora por 4 bits. En ciencias de computos utilizan el termino nibble, para indicar un caracter que es representado por 4 bits.  


Hoy en día en MD5 esta roto, lo que significa hay tecnicas para encontrar una colisión, que nos dan el resultado mas rapido que utilizando la fuerza bruta. Una colision 







Entre las funciones de hashing mas conocidas estan MD5, SHA2, RIPMED.

**use case #1  **  
Digamos que usted quiere la ultima version de Ubuntu en un archivo ISO. Entra en un website que un amigo le recomendo https://www.thepiratebay.org/ y ve en los comentarios un mensaje que dice _"No baje eso que contiene Malware"_ ¿Sera verdad? ¿Como lo podemos corroborrar? Bueno si tenemos el hashing emitido por los desarolladores de Ubuntu para ese archivo ISO y lo comparamos cuando bajemos el archivo, podemos saber sí ha sido alterado o no.

En este caso yo le instalo un programa gratutito a mí computadora llamado HashTab y verifico.







**use case #2  **  
Digamos que usted necesita crear un website Ej, Facebook , pero que no quiere que sus desarolladores y/o empleados, sepan la contraseña del usuario.

Lo websites usualmente lo que comparan **NO** es la contraseña del usuario para saber sí entra o no en la pagina, sino el hashing de la contraseña.


MD5 - 128 bits
RIPMED - 160 bits
Sha1 - 160 bits
Sha2 - 256 bits

A medida de mayor bits, mayor seguridad y mas tiempo se tarda la funcion. Por lo que en algunos casos los desarolladores escogen Sha1 teniendo disponibles otras funciones, tendiendo en cuenta que tienen que balancear, seguridad vs velocidad. ¿A quien le gusta una pagina lenta?




**use case #3  **  
SHA2 fue creada en Estado Unidos.
RIPMED fue creada en Europa.

Bitcoin utiliza **SHA2**(256bits), **RIPMED**(160bits) ambos en su proceso del blockchain, la razón facil, el autor del bitcoin piensa que es mas seguro depender de ambos que de uno solo.







Lo unico que me preocuopa un poco es que la historia nos has enseñado que todas esas funciones de hashing fueron "rotas" con el tiempo. Antes no habian muchos motivos economicos para romper las funciones de hashing ahora los hay de sobra, Que pasaria sí.... se rompe el SHA2 y el RIPMED160. En ese momento ¿Cuanto valdria un Bitcoin?   






Next you can update your site name, avatar and other options using the _config.yml file in the root of your repository (shown below).

![_config.yml]({{ site.baseurl }}/images/config.png)

The easiest way to make your first post is to edit this one. Go into /_posts/ and update the Hello World markdown file. For more instructions head over to the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) on GitHub.
