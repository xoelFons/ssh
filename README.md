# Clave púb y priv en SSH + Filezilla.

## 1. Crear las claves.

Para ello deberemos tener SSH instalado en nuestra máquina. Usaremos un comando para generar las claves. El comando es el siguiente:

*** $ ssh-keygen ***

Ahora iremos al direcotrio ** .ssh ** para ver que se han creado las dos claves, la pública (id_rsa.pub) y la privada (id_rsa).

## 2. Compartir la clave pública.

Cuando veamos que tenemos las dos claves, tendremos que pasar la clave pública al usuario de la máquina a la que queramos hacer ssh. Para ello, usaremos este comando:

*** $ ssh-copy-id [usuario]@[IP de la máquina] ***

Quedaría algo así:

*** $ ssh_copy_id admin@10.0.9.24 ***

Nos pedirá la contraseña del admin del equipo al que queremos conectarnos. Cuando la pongamos, ya está lista para la conexión mediante ssh.

## 3. Realizar conexión

Usaremos el comando *** $ ssh admin@10.0.9.24 *** para conectarnos a la máquina deseada, podremos crear y modificar archivos entre muchas cosas más.
