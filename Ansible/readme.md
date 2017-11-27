<h1>Configuración de Ansible<h1>

<p>Se Instalan y se configuran los siguientes servicios:</p>

*Apache
*Munin

<p>El primer paso es el siguiente:</p>

Se utiliza el siguiente comando para instalar el servidor Web.

ansible-playbook -i hosts apache.yml

<p>Segundo paso Instalar Munin</p>

Para instalar munin se debe utilizar el siguiente comando:

ansible-playbook -i hosts munin.yml
