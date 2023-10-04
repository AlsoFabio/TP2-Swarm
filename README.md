- El comando para crear el servidor apache es: 
```sh
docker build -t image_apache ./apache-datos
```
- El comando para crear el servidor node es: 
```sh
docker build -t image_node ./node-datos
```
- Para desplegar los servicios se utiliza el siguiente comando en la consola: 
```sh
docker stack deploy -c servicios.yml services
``` 
Donde servicios.yml es el archivo .yml con la configuracion para el despliegue y services es el nombre de los servicios.

- Para acceder al servicio de apache hay que situarse en:
```
http://localhost:8080
```
- Para acceder al servicio de node hay que situarse en:
```
http://localhost:8090
```