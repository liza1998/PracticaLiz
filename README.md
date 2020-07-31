Aplicacion web desarrollada con flask, conectada con MongoDB, se utilizo redis como base de datos y de igual forma  ejecutandose en Nginx.
## Instrucciones que se deben de llevar a cabo


1. Primero colocamos el comando siguiente para clonar el respositorio
```
$ git clone https://github.com/liza1998/PracticaLiz.git
```
2. Asi mismo se tiene que ocupar el comando para compilar el contenedor, como consiguiente se tiene que acceder a la carpeta donde este el archivo, luego ejecutar el siguiente comando.
```
$ sudo docker-compose up -d
```
3. Para iniciar el contenedor debes de escribir el siguiente comando. 
```
$ sudo docker-compose up
```
4. Colocarte en tu navegador colocare en la barra la dirección localhost:8181 podras visualizar funcionando la aplicacion flask
 
### Como ver los datos en mongoDB
1. Ver que los contenedores se estén ejecutando correctamete
```
$ sudo docker ps
```
2. Verificar cual es el ID del contenedor mongoDB lo copias y despues  se ejecuta comando
```
$ sudo docker exec -it <ID> bash
```
3. Enseguida colocas mongo, para entrar a la consola

```
Ingresar el comando para listar las bases de datos
$ show dbs

```
```
Este comando es para seleccionar la base que se desea 
$ use testdb
```
```
Para mostrar las colecciones y visualizarlas
$ show collections
```
```
Se utiliza este comando para visuslizar los registros
$ db.users.find().pretty()
```
```
Para salir de la consola de MongoDB 
$ exit

```
