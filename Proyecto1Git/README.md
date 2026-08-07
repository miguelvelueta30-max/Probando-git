# GUIA BASICA PARA USAR GIT DESDE CERO

### 1. CONFIGURACION INICIAL ( SOLO SE  HACE UNA VEZ)

git -- version       # verifica si git está instalado
git config --global user.name "tu nombre de git"   # Aquí agregas tu usuario
git config user.name        # Para checar si se guardó el usuario
git config --global user.email "tu correo"      # Para guardar correo (de preferencia el que usaste con git hub)
git config --global init.defaultBranch main     # Define la rama principal como main
git config global color.ui auto     # Activa los colores en la terminal
git config --list       # Muestra toda tu configuración actual

### 2. INICIAR Y CLONAR REPOSITORIOS
git init        # Inicializa un nuevo repositorio en tu carpeta actual
git clone https://github.com/usuario/repo.git       # Clona un repositorio remoto a tu pc por https
git clone git@github.com:usuario/repo.git       #clona un repositorio remoto por SSH, más seguro

### 3. FLUJO DE TRABAJO BASICO
git status      # Muestra el estado de tus archivos (modificados, listos, etc...)
git add archivo.txt     # Agrega un archivo especifico al área de preparación (staging)
git add . agrega todos los archivos modificados al staging
git commit -m " Mensaje descriptivo "       # guarda los cambios del staging en el historial local
git log     # Muestra el historial completo de commits
git log --oneline --graph --all     # Muestra el historial resumido y gráfico
git diff        # Muestra que cambiaste antes de hacer add
git diff --staged       # Muestra que cambiaste después de hacer add

### 4. TRABAJO CON RAMAS (BRANCHES)
git branch      # Lista todas las ramas locales 
git branch nombre-rama      # Crea una nueva rama
git checkout nombre -rama       # Te cambia a esa rama
git checkout -b nombre -rama        # Crea una rama y te cambia a ella en solo paso

