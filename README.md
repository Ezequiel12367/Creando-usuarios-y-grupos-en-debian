# Creando-usuarios-y-grupos-en-debian
para crear un grupo debemos entrar en modo root
al grupo lo llamaremos casa
groupadd casa
después verificamos que se halla creado
cat /etc/group

después que hayamos verificado le cambiaremos de nombre de casa a familia
groupadd --n familia casa

crearemos los usuarios que les pondremos los nombres de nuestros padres.
creamos el usuario de mama
useradd sonia 
creamos como usuarios nuestro nombre
useradd eezequiel

verificamos si se logró crear los usuarios
cat /etc/passwd

ahora crearemos una contraseña a nuestro usuario en el grupo de familia
passwd sonia
passwd eezequiel

ahora agregaremos los usurario que hemos creados al grupo de familia, los usuarios son. sonia, eezequiel
adduser sonia familia
adduser eezequiel familia
eso sería todo.

abreviado todos los pasos que hicimos anteriormente.  
groupadd casa
cat /etc/group
groupadd --n familia casa
creamos el usuario de mama
useradd sonia
useradd eezequiel 
cat /etc/passwd
passwd sonia
passwd eezequiel
adduser sonia familia
adduser eezequiel familia
esos serían los comandos para crear usuarios y grupos en Linux/debían
