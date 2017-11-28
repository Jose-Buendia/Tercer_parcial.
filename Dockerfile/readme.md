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

docker run -d -P --name munin_web_server -p 2221:22 -p 80:80 server:16.04

<h2>Tercer paso, Adicion de las llaves ssh</h2>

Para ello utilizamos el siguiente comando en nuestro terminal:

ssh -o StrictHostKeyChecking=no root@127.0.0.1 -p 2221 -i key.private hostname

<h2>Cuarto paso confirmacion</h2>

Realizar prueba de conexion a la maquina creada anteriormente

ssh root@172.168.0.1 -p 2221 -i ../key.private

Si la conexion se establece esta listo y se puede entrar a la configuración de Ansible.
