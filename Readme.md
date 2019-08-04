#Generamos nuestra imagen a partir de mi dockerfile

1. docker build -t devops . ==> ./docker build -t devops /d/CURSOS/DEVOPS/DEVOPS_2018/app_ejemplo/ (Crea la imagen con el nombre devops)

2. ./docker run -p 3000:3000 devops ==> corro mi imagen creada

3. ./docker kill id_container => salgo de un contenedor

4. Luego si hacemos un cambio en nuestro codigo volvemos a ejecutar el comando => docker build -t devops .

5. luego vuelvo a correr mi imagen pero en el background ./docker run -d -p 3000:3000 devops

6. Ahorra corro mis pruebas => docker run devops npm test