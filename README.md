# PROYECTO FINAL

# Descripción

  Este repositorio contiene la primera entrega de mi Proyecto de Fin de Grado, enfocado en la implementación de un entorno seguro utilizando herramientas como Docker, Suricata, Zeek, Python,     IPTables y otras soluciones para la detección y prevención de amenazas.

# Estructura del Repositorio:

  📂 src/        # Código fuente del proyecto
  
  📂 docs/       # Documentación del proyecto
  
  📂 configs/    # Archivos de configuración (Docker, Suricata, etc.)

  
  📂 scripts/    # Scripts útiles para automatización y despliegue

  
  📄 README.md   # Descripción general del proyecto

  
  📄 .gitignore  # Archivos a excluir del repositorio

  
  📄 LICENSE     # Licencia del proyecto

  

# Instalación y Uso

Requisitos

  - Docker
  - Docker Compose
  - Python 3.9+
  - Git
  

# Pasos de Instalación

1. Clonar el repositorio:
   git clone <URL_DEL_REPO>
   cd <NOMBRE_DEL_REPOSITORIO>

2. Construir y levantar los contenedores:
   docker-compose up --build

3. Acceder a los servicios:
    - Kibana: http://localhost:5601
    - Elasticsearch: http://localhost:9200
    - Suricata y Zeek: Integración en progreso
   
   
# Contribución

  Si deseas contribuir a este proyecto, abre un issue o un pull request con mejoras o sugerencias.

# Licencia

  Este proyecto está bajo la licencia MIT.

