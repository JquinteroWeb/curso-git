# Ver versión de Git:
```git --version```

# Ayuda de Git:
```git help```

# Ayuda especifica de un comando:
```git help <command>```

# Ejemplo: 
```git help commit```

# Configurar git:
```git --help config```

# Configuración global:
```git config --global user.name "<nombre>"```
```git config --global user.email "<email>"```
```git config --global init.defaultBranch <branch>```

# Listar la Configuración de git:
```git config --global -e```

# Inicializar repositorio de Git:
```git init```

# Ver estado de los documentos:
```git status```

# Agregar los documentos al seguimiento de git:

# Agregar todos los documentos:
1. ```git add .```
# Agregar uno en específico:
2. ```git add <name-path>```

# Quitar un archivo del seguimiento:
```git reset <name-path>```

# Hacer commit:
```git commit -m "<Nuestro mensaje>"``` 
# Para hacer commits con la nomencaltura convecional ir a esta web
https://www.conventionalcommits.org/

# Agregar archivos y hacer commit:
```git commit -am "<Nuestro mensaje>"```
# Ver los commits durante el tiempo:
```git log```

# Recuperar proyecto al último commit:
```git checkout -- .```

# Ver en que rama estoy trabajando:
```git branch```

# Cambiar nombre de las ramas:
```git branch -m <nombre-viejo> <nuevo-nombre>```
# Ejemplo:
```git branch -m master main```

# Agregar archivos de un mismo tipo que estén en la raíz del proyecto:
```git add *.<ext>```
# Ejemplos:
```git add *.html```
```git add *.css```
```git add *.jss```

# Agregar archivos de un mismo tipo que estén en una carpeta:
```git add *<carpeta>/.<ext>```
# Ejemplos:
```git add public/*.html```
```git add style/*.css```
```git add js/*.jss```

# NOTA: Cuando creamos una carpeta y esta no va contener ningún archivo git automáticamente la va a eliminar por esta razón es importante agregar un archivo especial llamado .gitkeep

# Agregar todos los archivos de una carpeta
```git add <carpeta>/```
# Ejemplos:
```git add css/```
```git add js/```
```git add public/```

# Tags 
*Crear tag
```git tag <nombre>```
*Crear tag con mensaje
```git tag -a <tag> -m "<Mensaje tag>"```
# Crear mis alias personalizados:
```git config --global alias.<mi-alias> "<acción>"```
# Ejemplos:
```git config --global alias.s "status --short"```
```git config --global alias.h help```

# Alias del profe Fernando Herrera:
```git config --global alias.lg "log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all"```\

# Diferencias en mi proyecto:
```git diff```

# valdiar diferencias en stage:
```git diff --stage```

# Actualizar mensajes de commit:
* ultimo commit
```git commit --amend -m "<Mensaje nuevo>"```

# Revertir commit:
```git reset --soft HEAD^<numero de commits antes>```
* Ejemplos: al commit anterior
```git reset --soft HEAD^1```
* Ejemplos: dos commits atras
```git reset --soft HEAD^2```

# Viajes en el tiempo con --soft
```git reset --soft <identificador del commit>```
* Ejemplo :
```git reset --soft 12312c3```

# Viajes en el tiempo con --mixed
* No elimina cambios peros vuelve a ese punto
```git reset --mixed <identificador del commit>```
* Ejemplo :
```git reset --mixed 12312c3```

# Viajes en el tiempo con --hard:
 
* Deja todo como estaba en ese commit.
```git reset --hard <identificador del commit>```
* Ejemplo :
```git reset --hard 12312c3```

# Referencias en orden cronologico (SUPER IMPORTANTE)
``` git reflog```

# Renombrar archivo:
```git mv <nombre viejo> <nombre nuevo>``` 
* Ejemplo
```git mv hola.html holas.html``` 

# Eliminar archivo:
```git rm <nombre>```

# Rebase
```git rebase -i HEAD~<numero de commits a gestionar>```
Esto nos abre una consola interactiva luego presionamos la letra a para empezar a edictar

# Repositorios remotos

* Agregar mi proyecto al repositorio remoto
```git remote add origin <URL>```

* Ver fuente remota
```git remote -v```

* Enviar mi proyecto y establecerlo por default
```git push -u origin <ramaname>```
* Enviar mi proyecto
```git push```

# Publicar tags en repositorio
```git push --tags```














