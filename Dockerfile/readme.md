<h1>Configuraciones básicas y creación de Dockers de prueba</h1>

<h2>Primer paso</h2>

Se debe construir un docker personalizado que incluya servidor openssh

Con el Dockerfile se contruira la imagen de los Dockers

Se usa el siguiente comando por consola:

<pre>
<code>  Docker build -t server:16.04
</code>
</pre>

<h2>Segundo paso, Despliegue</h2>

Se crean unas maquinas para el despliegue, en este caso se creará un servidor apache

Para ello usamos el siguiente comando:

