# Comandos básicos

## Configuración inicial

### Configuración de identidad

Lo primero que suele solicitar git es que añada una identidad, es decir, un nombre y un correo, para saber quién realizó un ```commit```.

```bash
#Su correo lo puede añadir con el comando:
git config user.email "su_email@email.com"

#Su nombre lo puede añadir con el comando:
git config user.name "Su nombre"
```


Existen etiquetas que ayudan a definir el alcance de la configuración, la que git usa por defecto es la local (que solo afecta al repositorio), pero también se pueden usar otras etiquetas, como ```--system``` (define el usuario de git a nivel del sistema, en todo repositorio de la máquina), ```--global``` (define el usuario de git a nivel del usuario del sistema, solo repositorios del usuario), ```--worktree``` (define el usuario de git a nivel del árbol de trabajo actual), ```--file <filename>``` (define el usuario de git a nivel de archivos especificos). 

```bash
#Correo para todos los repositorios en el sistema operativo que usted use:
git config --system user.email "su_email@email.com"

#Nombre para todos en el usuario del sistema operativo que usted use:
git config --global user.name "Su nombre"
```
