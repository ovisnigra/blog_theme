---
layout: post
title: "apuntes ruby"
comments: false
description: "apuntes ruby"
keywords: "apuntes, ruby"
---

# Apuntes de Ruby en el _jakranchu_

Pad : <https://pad.kefir.red/p/programando_en-Peras>

para configurar nuestras maquinas con ruby

https://gorails.com/setup/ubuntu/16.04

para cuando te atoras codeando

https://stackoverflow.com/

Por si te atoras instalando, puedes usarlo y aprenderlo en línea.

https://repl.it/languages/ruby

para instalar Ruby

```
sudo apt-get update
sudo apt install ruby git-core curl zlib1g-dev build-essential
libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3
libxml2-dev libxslt1-dev libcurl4-openssl-dev python-software-properties libffi-dev nodejs
```

## Ruby y tipos de Datos

- Strings
- Fixnum ( Integer y Float ) => Estos son datos númericos
- Booleans
- Arrays
- Hashes
- Symbols

## Definiendo variables

Deben empezar con una letra minúscula o un guión bajo _.

Deben estar formadas por letras, números y/o guiones bajos.

Por convención se estableció que deben ser llamadas de manera tal que definan su funcionalidad, escritas en minúsculas y separadas por _ .

```
flagX = false
last_name = "Ramírez"
cel_11 = 123456789
```

## Operadores
Relacionales:

    ==

    !=

Booleanos:

    &&

    ||

    !

## Ejemplos para ejecutarse en la consola de Ruby [irb]:

UNO
```
suma_uno = 4 + 7
suma_dos = suma_uno + 8
suma_dos == 19
```

DOS
```
multiplicacion = 6 * 5
division = multiplicacion / 5
operacion = division - 3
cadena = "Hola" * operacion
cadena == "HolaHolaHolaHola"
```

TRES
```
resta_uno = 3 -2
valor = "uno"
resta_dos = resta_uno - valor
resta_dos == 0
```

CUATRO

```

if ((number * 4) / 4) == (12 + 12 - number - 16)

puts "Es correcto"
else
  puts "Inténtalo de nuevo"
end

---


# Sesión 2

- correr en vim
- Sublime

    https://www.sublimetext.com/docs/3/linux_repositories.html#apt

    wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -

    sudo apt-get install apt-transport-https

    echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list

    sudo apt-get update

    sudo apt install sublime-text

-Documentación de Ruby
-Codecademy

    Tópicos

    a = 4

    a += 1

    a -= 2

    a *= 4

    Clases "Todo en Ruby es un Objeto"

    'Hola'.instance_of?(String)

    "hola".nil?

    print "¿Cuál es tu nombre?"

    first_name = gets.chomp

    print "¿Cuál es tu apellido? "

    last_name = gets.chomp

    print "¿De qué Estado eres? "

    city = gets.chomp

    print "¿Cuál es tu helado favorito? "

    flavor = gets.chomp

    puts "Tu nombre es #{first_name} #{last_name}, eres de #{city} y tu helado favorito es el de #{state}"

#

# primer programa de prueba

print "¿Cuál es tu nombre?"

first_name = gets.chomp

print "¿Cuál es tu apellido? "

last_name = gets.chomp

print "¿De qué ciudad eres? "

city = gets.chomp

print "¿Cuántos años tienes?"

age = gets.chomp

print "¿Cuál es tu helado favorito? "

flavor = gets.chomp

puts "Tu nombre es #{first_name} #{last_name}, eres de #{city} y tu helado favorito es el de #{flavor}"

# el signo de gato solo (#) se usa para comentarios.
# el signo de gato (#), seguido de llaves se usa para insertar las interpolaciones.
# Ejemplo: #{interpolación}
