# Estructura del proyecto:
VOTING_APP_V2/
│
├── __pycache__/                # Archivos compilados automáticamente por Python (generalmente ignorados en control de versiones)
│
├── templates/                  # Carpeta de plantillas HTML para renderizado con Flask
│   ├── dashboard.html          # Panel de control del usuario autenticado
│   ├── edit_profile.html       # Vista para editar el perfil del usuario
│   ├── login.html              # Formulario de inicio de sesión
│   ├── register.html           # Formulario de registro de usuarios
│
├── uploads/                    # Directorio (presumiblemente) para almacenar imágenes o archivos subidos por el usuario
│
├── app.py                      # Archivo principal de la aplicación Flask; punto de entrada del proyecto
├── config.py                   # Configuración general de la aplicación (como claves secretas, rutas de base de datos, etc.)
├── create_admin.py             # Script para crear un usuario administrador manualmente
├── forms.py                    # Declaración de formularios Flask-WTF usados para el login, registro, edición de perfil, etc.
├── models.py                   # Definición de modelos y relaciones de la base de datos (probablemente usando SQLAlchemy)
├── readme.md                   # Documento README con información del proyecto (instrucciones de uso, instalación, etc.)



# Si vamos a crear entorno virtual para las librerías del proyecto (lo que es alternativo en pruebas, pero seguro):

python -m venv venv
source venv/bin/activate  # para macOS/Linux
venv\Scripts\activate     # para Windows

---------------------------


pip install flask flask-sqlalchemy flask-login flask-wtf wtforms pymysql werkzeug flask-wtf
pip install requests


# Base de datos: crear solo la base de datos (las tablas las crea el script)
flask_auth
CREATE DATABASE voting_flask_db_project;


# Recordemos:
Paquete	            | Descripción
--------------------------------------------------------------------------
flask		        | Framework web en Python.
flask-sqlalchemy	| ORM para interactuar con MySQL.
flask-login		    | Manejo de sesiones y autenticación de usuarios.
flask-wtf		    | Integración de Flask con formularios WTForms.
wtforms		        | Manejo de formularios con validaciones.
pymysql		        | Conector para trabajar con MySQL en Python.
werkzeug		    | Manejo seguro de contraseñas y utilidades web.

# Carga de archivos:
pip install flask flask-sqlalchemy flask-login flask-wtf wtforms pymysql werkzeug flask-wtf
pip install flask-reuploads

# pip install pillow
para generar las imagenes del captcha

# exportación de los logs de cambios a Excel (formato .xlsx),
pip install openpyxl

# Instalar la librería para generar PDFs
pip install reportlab
