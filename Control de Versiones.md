# Documentación de Control de Versiones: Introducción a Git y GitHub
## Introducción
El control de versiones es una práctica esencial en el desarrollo de software moderno que permite rastrear y gestionar los cambios realizados en los archivos del proyecto. Git es uno de los sistemas de control de versiones más populares, mientras que GitHub es una plataforma basada en la nube que utiliza Git para facilitar la colaboración y el almacenamiento de repositorios.

Esta documentación proporciona una introducción a Git y GitHub, incluyendo comandos básicos y flujos de trabajo comunes.

## 1. ¿Qué es Git?
Git es un sistema de control de versiones distribuido que permite a los desarrolladores:

- Rastrear cambios en los archivos.
- Colaborar con otros desarrolladores de forma eficiente.
- Revertir cambios a versiones anteriores.
- Trabajar sin conexión.

Git almacena el historial de cambios en un repositorio local, lo que facilita el trabajo distribuido.

![github](https://cdn.dribbble.com/users/138252/screenshots/2389144/media/74f1da472943133d2a8898a7c93be44f.png)

## 2. ¿Qué es GitHub?
GitHub es una plataforma que complementa a Git ofreciendo:

- Repositorios alojados en la nube.
- Herramientas para colaborar en proyectos (pull requests, issues, wikis).
- Integración con CI/CD y otras herramientas de desarrollo.

GitHub facilita la colaboración en proyectos open-source y privados, proporcionando un entorno seguro y accesible para gestionar proyectos.

## 3. Instalación de Git

### En Windows:
- Descargar Git desde el [sitio oficial](https://git-scm.com/).
- Instalar el ejecutable y configurar las opciones deseadas.

### En macOS:
- Utilizar Homebrew:
    ```bash
    brew install git
    ```
### En Linux:
- Usar el gestor de paquetes correspondiente (ejemplo en Ubuntu/Debian):
    ```bash
    sudo apt update
    sudo apt install git
    ```

## 4. Configuración inicial
Después de instalar Git, se debe configurar el nombre de usuario y correo electrónico:

```bas
git config --global user.name "Tu Nombre"
git config --global user.email "tu_email@ejemplo.com"
```

## 5. Comandos básicos de Git
### Crear y clonar repositorios
- Inicializar un repositorio local:
    ```bash
    git init
    ```
- Clonar un repositorio remoto:
    ```bash
    git clone <URL_del_repositorio>
    ```

### Seguimiento de cambios
- Ver el estado de los archivos:
    ```bash
    git status
    ```

- Añadir archivos al área de preparación:
    ```bash
    git add <nombre_del_archivo>
    ```

- o para añadir todos los cambios:
    ```bash
    git add .
    ```

- Confirmar los cambios:
    ```bash
    git commit -m "Mensaje descriptivo"
    ```

### Sincronización con repositorios remotos
- Añadir un repositorio remoto:
    ```bash
    git remote add origin <URL_del_repositorio>
    ```

- Subir cambios al repositorio remoto:
    ```bash
    git push origin <rama>
    ```

- Actualizar desde el repositorio remoto:
    ```bash
    git pull origin <rama>
    ```
### Ramas
- Crear una nueva rama:
    ```bash
    git branch <nombre_de_la_rama>
    ```

- Cambiar a una rama existente:
    ```bash
    git checkout <nombre_de_la_rama>
    ```

- Fusionar ramas:
    ```bash
    git merge <rama_a_fusionar>
    ```

### Historial y registros
- Ver el historial de commits:
    ```bash
    git log
    ```

- Ver cambios en un archivo:
    ```bash
    git diff <nombre_del_archivo>
    ```

## 6. Flujo de trabajo básico con Git y GitHub
- Clonar el repositorio remoto:
    ```bash
    git clone <URL_del_repositorio>
    ```

- Crear una nueva rama para trabajar en una característica o corrección:
    ```bash
    git branch <nombre_de_la_rama>
    git checkout <nombre_de_la_rama>
    ```

- Realizar cambios y confirmarlos:
    ```bash
    git add .
    git commit -m "Descripción de los cambios realizados"
    ```

### Fusionar la rama con la rama principal (main):
- Cambiar a la rama principal:
    ```bas
    git checkout main
    ```
Fusionar los cambios:
    ```bash
    git merge <nombre_de_la_rama>
    ```
- Sincronizar con el repositorio remoto:
    ```bash
    git push origin main
    ```
## 7. Buenas prácticas
- Realizar commits con mensajes claros y descriptivos.
- Usar ramas para desarrollar nuevas características o solucionar problemas.
- Sincronizar frecuentemente con el repositorio remoto.
- Revisar y probar los cambios antes de fusionarlos.

## 8. Recursos adicionales
- [Documentación oficial de Git](https://git-scm.com/doc)
- [GitHub Learning Lab](https://docs.github.com/es/pages)
- Tutorial interactivo: [Try Git](https://trygit.js.org/)