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
