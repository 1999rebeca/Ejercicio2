# Ejercicio2

1. Creación de repositorio en GitHub, inicializándolo con un README.md y el .gitignore que GiHub ofrece para Java.
2. Modificación de este README.md desde GitHub para indicar lo dos primeros pasos.
3. Clono el repositorio
4. Creo un proyecto en ese directorio
5. ¡Ups! el proyecto se creó en una subcarpeta. Muevo su contenido al directorio raiz del repo.
6. Quiero volver al paso 3 para hacerlo bien. Hago un log


```
 a22rebecabo@W10N-I9E07 MINGW64 ~/Documents/contornos/Ejercicio Git2 (master)
$ git log --oneline
b0f65d7 (HEAD -> master) creando proyecto en intellij
ab3fec6 Update README.md
593deac Initial commit 
```

  Como quiero volver a antes de crear el proyecto, tengo que hacer un reset al commit previo (5ae4948). Al hacerlo, perdería los commits posteriores, así que creo una rama nueva para ello.

```
a22rebecabo@W10N-I9E07 MINGW64 ~/Documents/contornos/Ejercicio Git2 (master)
$ git branch rama2

a22rebecabo@W10N-I9E07 MINGW64 ~/Documents/contornos/Ejercicio Git2 (master)
$ git checkout rama2
Switched to branch 'rama2'
```

Ahora ya puedo hacer el reset:

```
a22rebecabo@W10N-I9E07 MINGW64 ~/Documents/contornos/Ejercicio Git2 (rama2)
$ git reset --hard ab3fec6a71021372720d5f0a054ef266c23ad914
HEAD is now at ab3fec6 Update README.md
```

y crear el proyecto directamente en el directorio donde ya está el repo.

![captura ejercicio git2](https://user-images.githubusercontent.com/114091264/203117287-45797ddc-276f-444a-b88b-c4b3e86f0dc1.png)

