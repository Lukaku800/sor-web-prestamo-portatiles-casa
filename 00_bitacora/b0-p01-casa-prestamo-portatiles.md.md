# b0-0.5.1 · Metodología y estructura

- **Alumno:** Lucas Chico
    
- **Bloque:** B0 — Prerrequisitos
    
- **Fase / ejercicio:** Fase 0.5.1 - Montar el Entorno en Casa
    
- **Fecha de inicio:** 26/10/2026
    
- **Fecha de entrega:** 26/10/2026
    

### 🎯 Qué se pedía

El objetivo de esta fase era dejar el ordenador de casa configurado con el mismo entorno de trabajo que el del instituto de una sola vez. Para ello, había que instalar Obsidian, Git y OBS, generar una nueva clave SSH específica para el equipo de casa, vinculada a GitHub, y reconstruir la estructura local de la bóveda clonando todos los repositorios personales desde GitHub.

### ⌨️ Comandos y pasos importantes

- `git version` — Para verificar que Git se ha instalado correctamente.
    
- `ssh-keygen -t ed25519 -C "tu-correo-de-github"` — Para generar una nueva clave SSH del tipo ed25519 para el ordenador de casa.
    
- `cat ~/.ssh/id_ed25519.pub` — Para mostrar por pantalla el contenido de la clave pública SSH y copiarla a GitHub.
    
- `git config --global user.name "Lucas Chico"` — Para establecer tu nombre globalmente en la configuración de Git.
    
- `git config --global user.email "tu-correo-de-github"` — Para vincular tu correo globalmente a la configuración de Git.
    
- `ssh -T git@github.com` — Para probar la conexión SSH con GitHub y comprobar que la autenticación es correcta.
    
- `mkdir -p RUTA_SOR/Boveda_SOR/00_Apuntes` — Para crear la carpeta de apuntes dentro de la estructura contenedora local fuera de OneDrive.
    
- `mkdir -p RUTA_SOR/Boveda_SOR/01_Practicas` — Para crear la carpeta donde irán los repositorios de las prácticas.
    
- `cd RUTA_SOR/...` — Para navegar a través del terminal hasta el directorio deseado.
    
- `pwd` — Para comprobar y confirmar la ruta actual donde estás ubicado en el terminal.
    
- `git clone git@github.com:TU-USUARIO/apuntes-sor-t1.git Trimestre_1` — Para clonar el repositorio de apuntes asignándole directamente el nombre de carpeta `Trimestre_1`.
    
- `git clone git@github.com:TU-USUARIO/bloque-0-prerequisitos.git B0_Prerrequisitos` — Para clonar el repositorio del Bloque 0 por SSH.
    
- `git clone git@github.com:TU-USUARIO/bloque-1-entorno.git B1_Entorno` — Para clonar el repositorio del Bloque 1 por SSH.
    
- `git clone git@github.com:TU-USUARIO/bloque-2-ubuntu-local.git B2_Ubuntu_Local` — Para clonar el repositorio del Bloque 2 por SSH.
    

### 🛠️ Qué he hecho

1. Preparé la grabación creando primero el fichero `b0-0.5.1-entorno-en-casa.md` vacío con la estructura requerida.
    
2. Inicié la grabación con OBS, me presenté indicando mi nombre (Lucas Chico), curso ($2.^{\circ}$ SMR) y fase, y mostré mi perfil de GitHub.
    
3. Instalé Obsidian, Git (asegurando marcar la opción "Open Git Bash here" en Windows) y OBS en mi equipo de casa.
    
4. Comprobé la instalación con `git version`.
    
5. Generé una clave SSH específica para mi ordenador de casa, copié la clave pública y la añadí a mi cuenta de GitHub con el título "Equipo Casa".
    
6. Configuré mi nombre y correo de GitHub en Git global y verifiqué la conexión con `ssh -T git@github.com`.
    
7. Creé la estructura de carpetas contenedora local para la bóveda fuera de la ruta de OneDrive.
    
8. Cloné mi repositorio de apuntes con el nombre de carpeta `Trimestre_1` en `00_Apuntes/`.
    
9. Cloné mis tres repositorios de prácticas (`B0_Prerrequisitos`, `B1_Entorno` y `B2_Ubuntu_Local`) dentro de `01_Practicas/`.
    
10. Abrí Obsidian con el botón _Open folder as vault_ apuntando a la carpeta `Boveda_SOR` y comprobé que la estructura fuera idéntica a la del centro.
    
11. Detuve la grabación, nombré el archivo de vídeo `B0.5.1 Montar el entorno en casa`, lo subí como "No listado" a la playlist `B0_Prerrequisitos` con sus respectivos timestamps y guardé el enlace.
    

### 🚩 Qué me ha fallado y cómo lo he resuelto

_(Si te ocurrió alguno de los errores indicados en la guía del PDF, puedes indicarlo aquí. Si no tuviste fallos, sustitúyelo por "nada")_:

- **Error / Problema:** Olvidé especificar el nombre de la carpeta al clonar los apuntes y la carpeta se creó como `apuntes-sor-t1`.
    
    - **Resolución:** Renombré la carpeta manualmente a `Trimestre_1` (o la volví a clonar especificando `.git Trimestre_1` al final).
        

### 🤔 Respuestas a las preguntas

1. **¿Por qué clonas desde GitHub en vez de copiar con pendrive?**
    
    Porque en GitHub se encuentra la versión buena y actualizada tras haberla subido desde el ordenador del centro. Clonar garantiza que la copia de casa sea exactamente idéntica a la del aula sin arrastrar desajustes.
    
2. **¿Por qué generas una clave SSH nueva en casa?**
    
    Porque las claves privadas nunca deben copiarse entre ordenadores. En cada equipo físico se genera una clave única y se añade la clave pública a GitHub para identificar ese dispositivo concreto.
    
3. **¿Dónde NO debe estar la bóveda?**
    
    La bóveda nunca debe ubicarse dentro de la carpeta de OneDrive ni en ubicaciones sincronizadas en la nube, ya que Git y OneDrive interfieren y se pelean entre sí generando conflictos y ficheros duplicados.
    

### 🔗 Enlaces

- **Vídeo de esta fase:** [https://youtu.be/7C6JqZM3cW0](https://youtu.be/7C6JqZM3cW0)
    
- **Playlist:** [https://www.youtube.com/playlist?list=PLRsAL-2PnyME](https://www.youtube.com/playlist?list=PLRsAL-2PnyME)
    

### 💭 Dudas / a repasar

- Repasar los pasos de sincronización pull y push entre el equipo del centro y el equipo de casa para mantener actualizados los apuntes.