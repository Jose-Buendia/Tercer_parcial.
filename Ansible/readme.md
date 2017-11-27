<h1>Configuración de Ansible</h1>

<p>Se Instalan y se configuran los siguientes servicios :</p>

Apache
Munin

<h1>El primer paso es el siguiente :</h1>

Se utiliza el siguiente comando para instalar el servidor Web.

ansible-playbook -i hosts apache.yml

<h1>Segundo paso Instalar Munin</h1>

Para instalar munin se debe utilizar el siguiente comando :

ansible-playbook -i hosts munin.yml
