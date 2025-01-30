# 📌 Curso de Git - Documentación  

Este repositorio está destinado al aprendizaje y práctica de **Git**, una herramienta de control de versiones ampliamente utilizada en el desarrollo de software.  

## 📖 Contenido del curso  

Durante el curso, se aprendieron los conceptos básicos de Git, incluyendo:  

- **Uso de la Git Shell**  
- **Comandos esenciales de Git**:  

  | Comando | Descripción |
  |---------|------------|
  | `git init` | Inicializa un nuevo repositorio Git. |
  | `git clone <URL>` | Clona un repositorio remoto. |
  | `git log` | Muestra el historial de commits. |
  | `git add <archivo>` | Agrega archivos al área de preparación (*staging*). |
  | `git commit -m "Mensaje"` | Guarda los cambios con un mensaje descriptivo. |
  | `git pull` | Descarga cambios del repositorio remoto. |
  | `git push` | Sube cambios al repositorio remoto. |
  | `git status` | Muestra el estado del repositorio y los archivos modificados. |

## 🔄 Comandos avanzados de Git  

### 🔍 `git diff`  
El comando `git diff` permite ver las diferencias entre archivos en distintas etapas del repositorio.  

| Comando | Descripción |
|---------|------------|
| `git diff` | Muestra las diferencias entre el directorio de trabajo y el área de preparación (*staging*). |
| `git diff --staged` | Muestra las diferencias entre el área de preparación y el último commit. |
| `git diff <commit1> <commit2>` | Compara los cambios entre dos commits específicos. |

### 🔄 `git restore`  
El comando `git restore` permite deshacer cambios en archivos no confirmados, restaurándolos a su estado anterior.  

| Comando | Descripción |
|---------|------------|
| `git restore <archivo>` | Restaura un archivo al último commit, descartando los cambios no guardados. |
| `git restore --staged <archivo>` | Quita un archivo del área de preparación (*staging*), pero mantiene los cambios en el directorio de trabajo. |
| `git restore .` | Restaura todos los archivos del directorio de trabajo a su versión más reciente en Git. |

⚠ **¡Cuidado!** Usar `git restore` puede descartar cambios no guardados. Si no quieres perderlos, haz un commit o guárdalos con `git stash`.  

## 🌿 Gestión de Ramas en Git  

En Git, las ramas (*branches*) permiten trabajar en diferentes versiones de un proyecto sin afectar la rama principal (`main`).  

### 📌 `git branch`  
El comando `git branch` se usa para listar, crear o eliminar ramas en Git.  

| Comando | Descripción |
|---------|------------|
| `git branch` | Muestra todas las ramas disponibles en el repositorio. |
| `git branch <nombre-rama>` | Crea una nueva rama sin cambiar a ella. |
| `git branch -d <nombre-rama>` | Elimina una rama que ya ha sido fusionada. |
| `git branch -D <nombre-rama>` | Fuerza la eliminación de una rama, incluso si tiene cambios sin fusionar. |

### 🔀 `git checkout -b <nombre-rama>`  
Este comando crea una nueva rama y cambia automáticamente a ella. Es equivalente a:  
```
git branch <nombre-rama>
git checkout <nombre-rama>
```

### 🔄 `git switch`
| Comando | Descripción |
|---------|------------|
| `git switch  <nombre-rama>` | Cambia a una rama existente. |
| `git switch -c <nombre-rama>` | Crea una nueva rama y cambia a ella (equivalente a `git checkout -b`). |


### 🔄 `git merge`  
El comando `git merge` se utiliza para fusionar los cambios de una rama a otra. Usualmente se fusionan las ramas de características (feature branches) en la rama principal (`main` o `master`).

| Comando                     | Descripción |
|-----------------------------|-------------|
| `git merge <rama>`           | Fusiona los cambios de la rama especificada a la rama actual. |
| `git merge --no-ff <rama>`   | Realiza una fusión sin hacer un "fast-forward", creando un commit de fusión explícito. |
| `git merge --abort`          | Si hay conflictos durante la fusión, puedes usar este comando para cancelar la operación de fusión y volver al estado anterior. |

#### ⚠ **Conflictos de fusión**  
Cuando Git no puede fusionar automáticamente las ramas debido a cambios conflictivos, se crea un conflicto de fusión. En este caso, debes resolver los conflictos manualmente en los archivos afectados.  
Una vez resueltos los conflictos, agrega los archivos con `git add` y luego haz el commit de la fusión con `git commit`.


## 🚀 Objetivo  
Este curso proporciona una base sólida para gestionar proyectos con Git de manera eficiente, permitiendo un mejor seguimiento de cambios y colaboración en equipo.  
---

📌 **Autor:** [Matias Paez]  
📅 **Última actualización:** [29/01/25]  

---

**Te invito a indagar más sobre el tema en :**

- **[atlassian](https://www.atlassian.com/es/git)**  

