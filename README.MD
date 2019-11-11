# Repositorio Git LFS
## Objetivo: poner en práctica el trabajo con repositorios LFS
------
*Pasos seguidos para esta práctica:*
1. Una persona del grupo crea el repositorio de Github.
2. Cada persona del grupo debe generar un par de claves SSH (ssh-keygen) y luego pasar la clave pública al propietario del repositorio.
3. El propietario del repositorio lo añade a claves permitidas con acceso a lectura y escritura.
4. Cada miembro hace "git init" en una carpeta vacía, luego "git install lfs" y luego recupera la información que pudiera haber en el repositorio remoto con "git pull origin master".
5. Como queremos que no se haga seguimiento de un tipo de archivo de imagen, por ejemplo, "bmp", lo ponemos en la lista de exclusión (.git/info/exclude).
6. Queremos que sí se haga seguimiento de "png" y "jpg" así que ponemos:
- git lfs track "\*.png"
- git lfs track "\*.jpg"
(va a ir dentro del .gitattributes, que solo haría falta hacerse una vez).
7. Finalmente, cada uno pone sus archivos, hace commit y los sube con git push.
