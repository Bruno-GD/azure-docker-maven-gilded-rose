<!-- 1- Crear una VM -->
## Crear una VM en Azure Cloud
###### Requisito previo, tener cuenta en Microsoft Azure
1. Acceder a la web de Azure (panel de control)
2. Crear una nueva Máquina virtual

![](docs/azure-main.png)

3. Rellenar los campos obligatorios para la creación de una VM

![](docs/azure-vm.png)

<!-- 2- Conectarse a ella -->
## Conectarse a nuestra VM de Azure Cloud

4. Visualizar la información de la VM para poder conectarnos

![](docs/azure-info.png)

5. Copiar la IP pública de nuestra máquina para poder conectarnos a través de SSH
6. Acceder a nuestro CLI para conectarnos con SSH _(en mi caso usaré PuTTY)_
7. Conectarse a la máquina con nuestro usuario y contraseña

![](docs/1.png)
<!-- 3- Instalar la paquetería necesaria en la VM -->
## Actualizar la lista de paquetes
8. Ejecutar los comandos `$ apt update | apt upgrade` <br><small>en caso de error usar `sudo`</small>

![](docs/2.png)
![](docs/3.png)

<!-- 4- Instalar git -->
## Instalación de paquetería necesaria
9. Instalar `git` con `$ sudo apt install git`

![](docs/4.png)

<!-- 5 - Instalar Docker (nivel ninja utilizando el script de bash obtenido de get-docker.com) -->
10. Instalar `docker` y `docker.io` con `$ sudo apt install docker.io`

![](docs/5.png)
![](docs/6.png)
###### Comprobación de git y docker instalados
![](docs/7.png)

<!-- 6 - Repetir los pasos de la en entrega del Gilded Rose dockerizada -->
## Crear contenedor de Docker y ejecutar el proyecto Maven
11. Clonar el repositorio con el proyecto Maven

![](docs/8.png)

12. Crear el contenedor con `docker build`

![](docs/9.png)

13. Ejecutar el contenedor con `docker run`

![](docs/10.png)