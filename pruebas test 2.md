https://github.com/oortega/testpr
git remote add upstream git@github.com:oortegawh/testpr.git
git remote -v

1.4 Actualizar repositorio local con los cambios del remoto upstream

git fetch upstream master
git merge upstream/master

[1] Subir los cambios de tu repositorio local al repositorio remoto forkeado

git push origin master


### primer caso

1.-agregue ignore y luis no va actalizar
2.-Luis subio pull linea 2 - Pull 1 y acepto pull. No ve el archivo .gitignore porque no actualizo
3.oscar actualizo antes del pull. no actualice el cambio de Luis y va hacer pull 2
   no me dejo subir porque detecta que no estoy actualizado
   Can’t automatically merge. Don’t worry, you can still create the pull request. 

   una vez que actualice ya me sale  Able to merge. These branches can be automatically merged.

4.-nene no actualio y hace pull 3
	le debe salir cant automatically merge - si le salio y debe actualizar su local contra el upstream, hacer merge con upstream y luego hacer push para el pull
	
	
	

## caso 2

archivo test2.txt
todos actualizamos
Nene Linea 1 -> Pull 1 
Luis linea 2 -> pull 2
Oscar linea 3 -> pull 3

1.-Acepte pull Nene y todo bien
2.-Al aceptar el pull de Luis, marca conflictos y pide resolver. Entonces no hay forma que sobreescriba los cambios del pull 2.2.-Tuve que resolver conflicto para aceptar el pull
3.-El pull 3, es el mismo problema de arriba
en este caso hicimos

## paso1
git checkout -b oortega-master master

-b: Crear una rama nueva basada en otra rama


git pull git://github.com/oortega/testpr.git master

Baja los cambios del repositorio remoto  de la rama master

## paso 1.2
reparo conflictos
git add -A
git commit -m "fix conflictos 1.2"


## Step 2: Merge the changes and update on GitHub.

git checkout master
git merge --no-ff oortega-master
git push origin master

al hacer push en automatico nos cierra el pull request

