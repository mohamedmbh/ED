# 😎 **Entorno de Desarrollo**
### Repositorio de prueba para **Entorno de Desarrollo**

***

## **GIT**
Permite controlar el proceso de creación de software llevando un registro exhaustivo de todos los cambios realizados.

<br>

## 1. Comandos básicos
### 📝 Crea un repositorio git
```console
git init
```
### ➕ Añade uno o más archivos al staging area
```console
git add <archivo>
```
### ✅ Crea un commit con una descripción
```console
git commit -m "descripción del commit"
```
### 🚀 Sube los cambios al repositorio remoto
```console
git push
```
### 🔍️ Comprueba las diferencias entre commits 
```console
git diff
```
<br>

# ☠️ 2. Eliminar commits
## 2.1 Eliminar el último commit
### 🚨 (Si no se han publicado los cambios)
### Si quiero mantener los cambios en mi repositorio local
```console
git reset --soft HEAD~1
```

### Si no quiero mantener los cambios en mi repositorio local
```console
git reset --hard HEAD~1
```

<br>

## 2.2 Eliminar commit específico
### 🚨 Para no hacer una masacre es necesario seguir los siguientes pasos:
1. Ejecuto `git log` para conocer el id del commit que quiero eliminar.
2. Ejecuto `git rebase -i <id_commit>` para eliminar el commit.
3. Se nos abrirá el editor y tendremos dos opciones:
- Eliminamos el commit que deseamos
- Cambiamos la palabra pick por la palabra drop

```console
git rebase -i <id_commit>
```


### 🔥 No me hago responsables de los errores 🔥
![](https://i.imgflip.com/40noj6.jpg)