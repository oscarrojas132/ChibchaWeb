# ChibchaWeb

![Logo de ChibchaWeb](ChibchaWeb/media/archivos/logo.jpg)

ChibchaWeb es una aplicación web desarrollada con Django que gestiona diferentes módulos como Cliente, Distribuidor y Empleado. Este proyecto está diseñado para facilitar la administración de datos y procesos relacionados con estas entidades.

## Estructura del Proyecto

La estructura principal del proyecto es la siguiente:


### Descripción de Carpetas y Archivos Principales

- **`manage.py`**: Archivo principal para ejecutar comandos de Django.
- **`chibchaweb_django/`**: Contiene la configuración principal del proyecto, incluyendo:
  - `settings.py`: Configuración del proyecto.
  - `urls.py`: Enrutamiento principal.
  - `templates/`: Plantillas HTML compartidas.
  - `static/`: Archivos estáticos como CSS, JavaScript e imágenes.

- **`Cliente/`**: Módulo que gestiona la lógica relacionada con los clientes.
  - `models.py`: Define los modelos de datos.
  - `views.py`: Contiene las vistas para manejar las solicitudes HTTP.
  - `validar_tarjeta.py`: Archivo específico para validación de tarjetas.

- **`Distribuidor/`**: Módulo que gestiona la lógica relacionada con los distribuidores.
  - `BancaryReportFacade.py`: Implementa la lógica para generar reportes bancarios.
  - `ReportAdapter.py`: Adaptador para reportes.
  - `XMLGenerator.py`: Generador de archivos XML.

- **`Empleado/`**: Módulo que gestiona la lógica relacionada con los empleados.

- **`Home/`**: Módulo para la página principal o funcionalidad general.

- **`media/`**: Carpeta para almacenar archivos subidos por los usuarios.

## Requisitos Previos

Antes de ejecutar la aplicación, asegúrate de tener instalados los siguientes requisitos:

- Python 3.x
- Un entorno virtual configurado
- Las siguientes dependencias de Python:

  ```plaintext
  asgiref==3.8.1
  chardet==5.2.0
  Django==5.1.7
  djangorestframework==3.15.2
  mysqlclient==2.2.7
  pillow==11.1.0
  reportlab==4.3.1
  sqlparse==0.5.3
  tzdata==2025.2

## Instalación

1. Clona este repositorio:

   ```bash
   git clone https://github.com/oscarrojas132/ChibchaWeb.git
   cd ChibchaWeb

2. Crea un entorno virtual e instálalo:

    ```bash
    python -m venv venv
    source venv/bin/activate  # En Windows: venv\Scripts\activate
    cd ChibchaWeb
    pip install -r requirements.txt

3. Configura la base de datos en

    ```bash
    chibchaweb_django/settings.py

4. Aplica las migraciones:

    ```bash
    python manage.py migrate

5. Ejecuta el servidor de desarrollo:

    ```bash
    python manage.py runserver


Uso
Accede a la aplicación en tu navegador en http://127.0.0.1:8000/.

Tests
Para ejecutar los tests, usa el siguiente comando:

    ```bash
    python manage.py test
    
## Capturas de Pantalla

### Página Principal
![Página principal](ChibchaWeb/media/archivos/Captura%20de%20pantalla%202025-03-25%20095230.png)

### Panel de Control de un Usuario
![Panel de administración](/ChibchaWeb/media/archivos/Captura%20de%20pantalla%202025-03-25%20100204.png)