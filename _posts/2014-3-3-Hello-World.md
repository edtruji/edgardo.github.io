---
layout: post
title: Hashing 101
---

El hashing es una función matematica en la cual le damos un **INPUT**, y nos devuelve un **OUTPUT** fijo del mismo tamaño y unico para ese **INPUT** en especifico. Ese **INPUT** pudiera ser una imagen, un audio, una contraseña.

Digamos que tenemos la contraseña **123Abc**, y tenemos la contraseña **123abc**

MD5 123Abc -> **876dfefef3ef6f4548f48bbddd856cef**
MD5 123abc -> **a906449d5769fa7361d7ecc6aa3f6d28**

Lo que significa que la funciones de hashing son case-sensitive, cuaquier cambio de mayusculas a minusculas cuenta.
En el caso de MD5, nos devuelve un largo fijo de 128 bits, pero sí contamos la cantidad de caracteres nos fijamos que tenemos 32.
32 x 4 = 128 bits. El **OUTPUT** de MD5 no es un "STRING" sino mas bien caracteres hexadecimales, cada caracter hexadecimal (0-9)(A-F) es representado en la computadora por 4 bits.






Entre las funciones de hashing mas conocidas estab MD5, SHA2, RIPMED.

use case #1
use case #2
use case #3














Next you can update your site name, avatar and other options using the _config.yml file in the root of your repository (shown below).

![_config.yml]({{ site.baseurl }}/images/config.png)

The easiest way to make your first post is to edit this one. Go into /_posts/ and update the Hello World markdown file. For more instructions head over to the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) on GitHub.
