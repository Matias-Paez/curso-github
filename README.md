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


## 🚀 Objetivo  
Este curso proporciona una base sólida para gestionar proyectos con Git de manera eficiente, permitiendo un mejor seguimiento de cambios y colaboración en equipo.  

---

📌 **Autor:** [Matias Paez]  
📅 **Última actualización:** [29/01/25]  
