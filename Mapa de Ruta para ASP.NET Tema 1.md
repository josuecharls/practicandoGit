# Unidad I: Habilidades Generales del Desarrollador

## Tema 1: GIT - Control de Versiones (VSTS, GitHub, GitLab)

Git es un sistema de control de versiones distribuido que te permite rastrear cambios en el c�digo fuente durante el desarrollo de software. Es una herramienta esencial para cualquier desarrollador. A continuaci�n, te proporcionar� una explicaci�n did�ctica y ejercicios para que puedas practicar.

### Conceptos B�sicos de Git

1. **Repositorio (Repo)**: Un lugar donde se almacena el c�digo y el historial de cambios.
2. **Commit**: Un registro de cambios realizados en el repositorio.
3. **Branch (Rama)**: Una l�nea paralela de desarrollo.
4. **Merge**: Combina cambios de diferentes ramas.
5. **Clone**: Copia un repositorio existente.

### Ejercicios Pr�cticos

#### Ejercicio 1: Configuraci�n Inicial

```bash
# Configura tu nombre de usuario y correo electr�nico
git config --global user.name "Tu Nombre"
git config --global user.email "tuemail@example.com"
```

#### Ejercicio 2: Crear un Nuevo Repositorio

```bash
# Crea un nuevo directorio y navega a �l
mkdir mi_proyecto
cd mi_proyecto

# Inicializa un nuevo repositorio Git
git init
```

#### Ejercicio 3: Realizar tu Primer Commit

```bash
# Crea un nuevo archivo
echo "# Mi Proyecto" > README.md

# A�ade el archivo al �rea de preparaci�n
git add README.md

# Realiza un commit
git commit -m "Primer commit - A�adir README.md"
```

#### Ejercicio 4: Crear y Fusionar Ramas

```bash
# Crea una nueva rama
git checkout -b nueva_rama

# Realiza cambios en la nueva rama
echo "Contenido en la nueva rama" > archivo.txt
git add archivo.txt
git commit -m "A�adir archivo.txt en nueva_rama"

# Cambia a la rama principal (main)
git checkout main

# Fusiona la nueva rama con la rama principal
git merge nueva_rama
```

#### Ejercicio 5: Clonar un Repositorio

```bash
# Clona un repositorio existente desde GitHub
git clone https://github.com/usuario/repositorio.git
```

### Uso de GitHub

GitHub es una plataforma de alojamiento para proyectos que utiliza Git. Te permite colaborar con otros desarrolladores, revisar el c�digo, y gestionar proyectos.

#### Ejercicio 6: Crear un Repositorio en GitHub

1. Ve a [GitHub](https://github.com/) y crea una cuenta si a�n no tienes una.
2. Haz clic en el bot�n "New" para crear un nuevo repositorio.
3. Nombra tu repositorio y selecciona las opciones deseadas.
4. Sigue las instrucciones para conectar tu repositorio local con GitHub.

#### Ejercicio 7: Subir Cambios a GitHub

```bash
# A�ade la URL del repositorio remoto
git remote add origin https://github.com/usuario/repositorio.git

# Empuja los cambios a GitHub
git push -u origin main
```

### Uso de GitLab

GitLab es otra plataforma popular para alojar proyectos Git.

#### Ejercicio 8: Crear un Repositorio en GitLab

1. Ve a [GitLab](https://gitlab.com/) y crea una cuenta si a�n no tienes una.
2. Haz clic en el bot�n "New Project" para crear un nuevo repositorio.
3. Sigue las instrucciones para conectar tu repositorio local con GitLab.

#### Ejercicio 9: Subir Cambios a GitLab

```bash
# A�ade la URL del repositorio remoto
git remote add origin https://gitlab.com/usuario/repositorio.git

# Empuja los cambios a GitLab
git push -u origin main
```

### Uso de VSTS (Azure DevOps)

Azure DevOps es una plataforma de Microsoft que proporciona herramientas para el desarrollo de software, incluyendo repositorios Git.

#### Ejercicio 10: Crear un Repositorio en Azure DevOps

1. Ve a [Azure DevOps](https://dev.azure.com/) y crea una cuenta si a�n no tienes una.
2. Crea un nuevo proyecto y selecciona la opci�n de repositorio Git.
3. Sigue las instrucciones para conectar tu repositorio local con Azure DevOps.

#### Ejercicio 11: Subir Cambios a Azure DevOps

```bash
# A�ade la URL del repositorio remoto
git remote add origin https://dev.azure.com/usuario/proyecto/_git/repositorio

# Empuja los cambios a Azure DevOps
git push -u origin main
```