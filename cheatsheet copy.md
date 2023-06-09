# CHEATSHEET

## configuración básica de usuario
- Configurar Nombre que salen en los commits  
 `git config --global user.name "Pool Hijuela"`   
- Configurar Email  
 `git config --global user.email "poolpetterhijuel@hotmail.com"`

## iniciando repositorio
- Iniciamos GIT en la carpeta donde esta el proyecto  
`git init`  
- Clonamos el repositorio de GitHub  
`git clone <url>`  
- Añadimos todos los archivos para el commit  
`git add .`  
- Hacemos el primer commit  
`git commit -m "mensaje"`  
- Subimos al repositorio  
`git push origin master`

## clonar repositorio
- Clonamos el repositorio de GitHub  
`git clone <url>`  

## git add
- Añadimos todos los archivos para el commit  
`git add .`  
- Añadimos el archivo para el commit  
`git add <archivo>`  
- Añadimos todos los archivos para el commit omitiendo los nuevos  
`git add --all `  
- Añadimos todos los archivos con la extensión especificada  
`git add *.txt`  
- Añadimos todos los archivos dentro de un directorio y de una extensión especifica  
`git add docs/*.txt`  
- Añadimos todos los archivos dentro de un directorios  
`git add docs/`

## git commit
Cargar en el HEAD los cambios realizados
```ssh
	git commit -m "Texto que identifique por que se hizo el commit"
```
Agregar y Cargar en el HEAD los cambios realizados
```ssh
	git commit -a -m "Texto que identifique por que se hizo el commit"
```
De haber conflictos los muestra
```ssh
	git commit -a 
```
Agregar al ultimo commit, este no se muestra como un nuevo commit en los logs. Se puede especificar un nuevo mensaje
```ssh
	git commit --amend -m "Texto que identifique por que se hizo el commit"
```
## GIT PUSH

Subimos al repositorio
```ssh
	git push <origin> <branch>
```
Subimos un tag
```ssh
	git push --tags
```
## GIT LOG

Muestra los logs de los commits
```ssh
	git log
```
Muestras los cambios en los commits
```ssh
	git log --oneline --stat
```
Muestra graficos de los commits
```ssh
	git log --oneline --graph
```
## GIT DIFF

Muestra los cambios realizados a un archivo
```ssh
	git diff
	git diff --staged
```

## GIT REMOTE

Agregar repositorio remoto
```ssh
	git remote add origin <url>
```
Cambiar de remote
```ssh
	git remote set-url origin <url>
```
Remover repositorio
```ssh
	git remote rm <name/origin>
```
Muestra lista repositorios
```ssh
	git remote -v
```
Muestra los branches remotos
```ssh	
	git remote show origin
```
Limpiar todos los branches eliminados
```ssh
	git remote prune origin 
```
## GIT BRANCH

Crea un branch
```ssh
	git branch <nameBranch>
```
Lista los branches
```ssh
	git branch
```


## OTROS COMANDOS

Lista un estado actual del repositorio con lista de archivos modificados o agregados
```ssh
	git status
```
Quita del HEAD un archivo y le pone el estado de no trabajado
```ssh
	git checkout -- <file>
```
Crea un branch en base a uno online
```ssh
	git checkout -b newlocalbranchname origin/branch-name
```
Busca los cambios nuevos y actualiza el repositorio
```ssh
	git pull origin <nameBranch>
```
Cambiar de branch
```ssh
	git checkout <nameBranch/tagname>
```
Une el branch actual con el especificado
```ssh
	git merge <nameBranch>
```
Verifica cambios en el repositorio online con el local
```ssh
	git fetch
```
Borrar un archivo del repositorio
```ssh
	git rm <archivo> 
```

