# Políticas de contraseñas

## Introducción

La seguridad de nuestro sistema puede verse amenazada por un uso incorrecto de las contraseñas.

El objetivo de la práctica es entender y configurar las directrices de seguridad, para ello utilizaremos el módulo pam pw_password.

## Desarrollo

* Instalación:

    Para instalar el paquete pam tan solo debemos introducir en una terminal de Linux: "sudo apt-get install libpam-cracklib"

* Configuración:
    /etc/security/pw_password.conf

    Dentro de dicho archivo podemos configurar la normativa de contraseñas, por ejemplo, editando la línea "ucredit = 0" podemos cambiar el número maximo de carácteres en mayuscula que pueda contener la contraseña, (si queremos establecer el mínimo, deberemos usar números negativos)

## Comprobación

Para comprobar si los cambios se han aplicado podemos utilizar el comando passwd, para crear una contraseña, en caso de no cumplir uno de los criterios especificados, el sistema nos lo mostrará a través de un mensaje

Si queremos ver todos los valores aplicados deberemos usar el comando: "sudo chage -l [usuario]"

# Políticas de contraseñas

