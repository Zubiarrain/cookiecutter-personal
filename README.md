# Pasos para el curso

### Crear carpeta del proyecto

``` bash
mkdir cookicutter-personal
cd cookicutter-personal
```

### Agregar canal a conda
``` bash
conda config --ad channels conda-forge
```

### Crear nuevo entorno con cookiecutter instalado
``` bash
conda create --name cookiecutter-personal cookiecutter=1.7.3
```

### Activar nuevo entorno
``` bash
conda activate cookiecutter-personal
```

### Crear archivo enviroment.yml que contiene los paquetes de ese entorno
``` bash
conda env export --from-history --file enviroment.yml
```

### Crear archivo enviroment.yml que contiene los paquetes de ese entorno
``` bash
conda env export --from-history --file enviroment.yml
```

# Crear esquema de archivos
![esquema de archivos](https://static.platzi.com/media/user_upload/Selection_999%28161%29-e0efc6c6-913e-4bd8-a90e-b380d54d968d.jpg)

- En el archivo cookiecutter.json se colocarán las variables que el usuario que quiera replicar el esquema debe completar al iniciar el cookicutter

- Se utiliza el lenguaje jinja ({{}}) para colocar variables. Por ejemplo el nombre de la carpeta principal es {{ cookiecutter.project_slug }}. la variable project_slug será completada por el usuario y la carpeta tomará ese nombre

### Hooks

