# Tarea 2 SXE
## Angel Jose Piñeiro Andion

### La siguiente práctica es una lista de tareas que tenéis que hacer. Por cada tarea tenéis que ir poniendo los comandos utilizados y, brevemente, describir el proceso.

### Crear un readme con mark down con las descripciones (un commit por cada apartado)

### Entregar el repositorio

### Utilizaremos la imagen de Alpine. Sigue las instrucciones:

### 1. Descarga la imagen "alpine" SIN ARRANCARLA y comprueba que está en tu equipo
En primer lugar descargamos la imagen de alpine con el siguiente comando.

    ```docker pull alpine```

Comprobamos que la imagen se ha descargado correctamente con el siguiente comando.

    ```docker images```
![apartado1.png](images/apartado1.png)
### 2. Crea un contenedor sin ponerle nombre. ¿está arrancado? Obtén el nombre
Creamos un contenedor sin nombre con el siguiente comando.

    ```docker run -it alpine```

Comprobamos que el contenedor se ha creado correctamente con el siguiente comando.

    ```docker ps -a```

Obtenemos el nombre del contenedor con el siguiente comando.

    ```docker ps -a --format "{{.Names}}"```
![apartado2.png](images/apartado2.png)
### 3. Crea un contenedor con el nombre 'dam_alp1'. ¿Como puedes acceder a él?
Creamos un contenedor con el nombre 'dam_alp1' con el siguiente comando.

    ```docker run -it --name dam_alp1 alpine```

Accedemos al contenedor con el siguiente comando.

    ```docker exec -it dam_alp1 /bin/sh```
![apartado3.png](images/apartado3.png)
