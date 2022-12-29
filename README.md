# Tutorial uso de git


<p align="center">
<img src="https://www.solucionex.com/sites/default/files/posts/imagen/git.jpg" style="max-width: 100%; display: inline-block;" />
</p>

## Apéndice

- Configurar git

- Inicializar repositorio

- Comandos útiles

- Realizar un commit

- Eliminar un archivo

- Restaurar un archivo

- Ver ramas

- Crear una rama

- Cambiar de rama

- Combinar ramas

- Conectar con Github




## Contenido

- Configurar git: 
 

git config --global user.name "Nahuel Garrido"

git config --global user.email garridonahuel8@gmail.com

    - --global indica que la configuración se debe efectuar globalmente y no únicamente en el proyecto que nos encontramos actualmente

- Inicializar repositorio:

Para inicializar un repositorio debemos utilizar el comando:

git init 

    - Genera un repositorio vacío en la carpeta que nos encontremos

- Comandos útiles:

git status

    - Muestra el estado actual del repositorio

git add archivo.txt

    - Agrega los cambios y/o el archivo a nuestra siguiente confirmación

git log

    - Muestra el historial de confirmaciones.


- Realizar un commit:

git commit -m "mensaje"

Antes de realizar un commit debemos revisar el estado del repositorio para evitar errores.

    - Confirma los cambios en la instancia

- Eliminar un archivo:

rm archivo.txt

    - Luego se debe agregar el archivo a nuestra confirmación y confirmar los cambios en la instancia.

Otra alternativa:

git rm archivo.txt

    - Elimina el archivo sin necesidad de confirmación
    
- Restaurar un archivo:

git restore archivo.txt

    - Nos permite recuperar archivos eliminados incluso, desde una etapa antes de hacer commit.


- Ignorar un archivo:

Se debe crear un archivo con el nombre ".gitignore"


    - Dentro de este archivo se escriben los nombres del archivo y/o carpeta a ignorar: 
    ejemplo: archivo.txt carpeta/

    - Se considera una buena práctica agregar este archivo a nuestra instancia

## Ramas

<p align="center">
<img src="https://www.pngitem.com/pimgs/m/194-1949056_git-merge-branch-hd-png-download.png" style="max-width: 100%; display: inline-block;" />
</p>

- Ver ramas:

git branch

    - Muestra las ramas y en la que te encuentras


- Crear una rama:

git checkout -b features/nombre-de-la-funcionalidad

    - Se considera una buena práctica escribirlo de esta forma o con el ticket de la feature.

- Cambiar de rama:

git checkout nombre

    - Nos permite movernos a la rama nombre

- Combinar ramas:

git merge nombre

    - Si queremos combinar una rama con nuestra rama main debemos ejecutar git merge nombre desde la rama main
    
- Borrar rama:

Si queremos borrar una rama debemos utilizar: git branch -d nombre

## Conectar con Github

Se debe crear un repositorio en github

git remote add origin https://github.com/nahugarrido/name.git

git push -u remote local

    - remote es la rama remota a la que subimos nuestra rama local 
    
    
    - Al crear el repositorio se nos muestra una guia de que debemos hacer para conectarlo con nuestro repositorio local


