pbsl
====

Python Barranquilla - Fundacion Software Libre de Colombia

Primera Clase
=============

1. Crear cuenta de Github.
2. Descargar GIT para su sistema operativo
3. Configurar el equipo: https://help.github.com/articles/set-up-git
4. Crear un 'fork' del repositorio de pbsl.
5. Clonar el repositorio:
    git clone https://github.com/tuusario/pbsl.git
6. Agregar el remote de fslcolombia.
    git remote add fslcol https://github.com/fslcolombia/pbsl.git
7. Correr el hola mundo:
    pyhton hola.py

Segunda Clase
=============

0. Linux (no es obligacion, pero recomendado para acelerar la clase)
1. Notebook de iPython:
   http://www.introtopython.org
2. Entorno de desarrollo recomendado: PyCharm.
   http://www.jetbrains.com/pycharm/

Tercera Clase
=============

Ya todos tenemos lo básico instalado y entendemos los conceptos fundamentales del lenguaje.

Ahora empecemos nuestra primera aplicación, usando programación basada en eventos vamos a estudiar aplicaciones web desde la capa más baja.

0. Corremos el servidor:
   '''
   cd code
   python server.py
   '''
1. Probamos que devuelve "En la 38" usando el explorador con la url http://localhost:9000/
2. Probamos conectando con telnet y con curl
   telnet 127.0.0.1 9000
   GET /

   curl http://127.0.0.1/
3. Corremos apache benchmark para probar cuantos requests nos responde por segundo en nuestra maquina:
   ab -c 2 -n 10000 http://127.0.0.1:9000/
