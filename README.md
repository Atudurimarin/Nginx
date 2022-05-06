# Nginx
Práctica instalación Nginx en Ubuntu

## Instalación Nginx
### 1 Instalación de la aplicación.
<br>

Procedemos a instalar la aplicación realizando un apt-get install nginx.  <br> <br>

![1](https://user-images.githubusercontent.com/91564326/167170882-d0e71323-1ef1-403a-8a71-a311a3faea83.png)<br> <br> 

Abrimos el navegador, introducimos localhost y si hemos instalado el Nginx correctamente nos aparece la página de inicio del servidor.<br> <br><br>

### 2 Comprobación de la correcta instalación. <br><br>
![3](https://user-images.githubusercontent.com/91564326/167171138-d07c96b9-289f-4679-88b6-eaad4b50c9d0.png)<br> <br> <br>

### 3 Sites-available y Sites-enabled. <br><br>
![4](https://user-images.githubusercontent.com/91564326/167171437-478c9908-6ece-4485-a31b-24d753a77ecc.png)<br> <br>

Podemos observar que existen dos directorios llamados sites-available y sites-enabled. <br> <br> <br>

### 4 Creación de los archivos pagina.web1.com y archivos pagina.web2.com . <br><br>
![5](https://user-images.githubusercontent.com/91564326/167171740-3e7045a6-55bb-4f21-827d-366e5b93c4d2.png)<br><br>
Dentro de la carpeta sites-available encontramos el archivo default, lo procedemos a copiar y crearemos dos archivos nuevos y los llamaremos como el dominio de cada una de las 2 webs que alojaremos.<br><br><br>

### 5 Configuración de los sitios.<br><br>
![6](https://user-images.githubusercontent.com/91564326/167171849-b3a621a2-ec8c-470d-ac7e-313bb56ed56f.png)
  <br><br>
Entramos en cada uno de los sitios que hemos creado y borramos el default server, cambiamos el nombre del servidor y el nombre del root.<br><br>

![7](https://user-images.githubusercontent.com/91564326/167171908-4bb957c9-2d3a-469e-9ffe-cfd977a36fc1.png)
  <br><br><br>

### 6 Creamos links de los archivos en sites-enabled.<br><br>
![8](https://user-images.githubusercontent.com/91564326/167171962-9fa7df92-216a-4919-8e04-3c3335dfc7cb.png)
  <br><br>
Creamos links de los archivos que hemos creado en sites-available para que la máquina pueda enlazarlos desde sites-enabled.<br><br><br>

### 7 Reiniciamos Nginx.<br><br>
![9](https://user-images.githubusercontent.com/91564326/167171994-7ce41398-95f5-44ab-ad36-c6ff2177f439.png)
  <br><br>
Reiniciamos Nginx con el comando nginx -s reload para que los cambios surtan efecto.<br><br><br>

### 8 Introducimos la IP de nuestro servidor.<br><br>
Entramos en /etc/hosts e introducimos la dirección IP a la que apuntarán los dos dominios que hemos creado.<br><br><br>
### 9 Creamos Directorios y archivos html.
<br><br>
Creamos los directorios con los nombres que habíamos creado en el root y dentro creamos el archivo index.html .
<br><br><br>

### 10 Creamos el archivo html.
<br><br>
![14](https://user-images.githubusercontent.com/91564326/167172344-9dcbfa50-ad48-4edb-b64b-9875847f52e6.png)
  <br><br>
Usamos el vim para modificar el archivo index.html e introducimos el código html de nuestra web.<br><br>
![11](https://user-images.githubusercontent.com/91564326/167172394-13c9bf7a-3ab4-46e1-a82c-6f36c8f27477.png)
<br><br><br>

### 11 Abrimos la web en nuestro navegador.<br><br>
![12](https://user-images.githubusercontent.com/91564326/167172449-badcaa65-5701-4d2a-a76d-f27625ec1e15.png)<br><br>
Si escribimos el dominio de nuestra web en la barra de direcciones del navegador, nos aparecerá el contenido de nuestras webs.<br><br>
![13](https://user-images.githubusercontent.com/91564326/167172523-c738ff87-7949-43c5-805b-05de9cd32547.png)
<br><br>





