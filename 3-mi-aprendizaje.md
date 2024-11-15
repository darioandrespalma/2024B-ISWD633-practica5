# COMPLETAR  
Comparando sus conocimientos antes de hacer la práctica con sus conocimientos después de hacer la tarea, explicar los principales aprendizajes logrados para beneficio de su formación profesional.  
Si solucionó un problema presentado al realizar la práctica también se debe documentar.

Antes de realizar la práctica de configuración de SonarQube y PostgreSQL con Docker Compose, mis conocimientos sobre la herramienta Docker Compose y su uso para orquestar múltiples contenedores eran generales. Sabía cómo crear servicios básicos y definir volúmenes y redes, pero tenía una experiencia limitada en la implementación de soluciones más complejas que requieren múltiples servicios y configuraciones específicas de bases de datos y aplicaciones.

### Aprendizajes:
1. **Configuración Compleja de Servicios**: Aprendí cómo configurar múltiples servicios con dependencias, como SonarQube y PostgreSQL, dentro de un archivo `docker-compose.yaml`. Entender cómo se enlazan los servicios mediante redes y cómo se configuran variables de entorno para la conectividad fue un avance significativo.

2. **Uso de Volúmenes**: Descubrí cómo definir y utilizar volúmenes persistentes para almacenar datos de forma que estos persistan entre reinicios de los contenedores. Esto es clave para mantener la integridad de los datos de bases de datos y aplicaciones como SonarQube.

3. **Configuración de Healthchecks**: La práctica me permitió profundizar en la configuración de `healthchecks`, lo que es esencial para garantizar que los servicios estén en un estado saludable antes de permitir que otros servicios dependan de ellos. Aprendí cómo ajustar parámetros como el `interval`, `timeout`, y `retries` para diferentes tipos de servicios.

4. **Mapeo de Puertos y Accesibilidad**: Reforcé mis conocimientos sobre cómo mapear puertos del host al contenedor para permitir la accesibilidad externa, como acceder a SonarQube desde `localhost:9000`.

5. **Interdependencia de Servicios**: Me familiaricé con el uso de `depends_on` y cómo garantizar que un servicio como SonarQube se inicie solo después de que PostgreSQL esté en un estado saludable.

### Solución de Problemas:
Durante la práctica, me encontré con un problema en el que SonarQube no se conectaba a PostgreSQL, arrojando errores de conexión. La solución requirió:
- Revisar los logs de los contenedores (`docker logs <container_name>`) para identificar el problema.
- Confirmar que las variables de entorno en el archivo `docker-compose.yaml` fueran correctas y estuvieran bien escritas.
- Asegurarme de que el contenedor de PostgreSQL estuviera corriendo y accesible en la red definida.

Este proceso de solución de problemas mejoró mis habilidades de depuración y mi capacidad para analizar mensajes de error de los contenedores, lo cual es fundamental para mi desarrollo profesional en el ámbito de DevOps y la administración de sistemas.

### Beneficio para la Formación Profesional:
La práctica consolidó mi comprensión sobre la orquestación de servicios en Docker Compose, algo que es vital para gestionar aplicaciones en contenedores de manera efectiva. También me proporcionó una mejor perspectiva sobre cómo implementar servicios complejos con dependencias y garantizando la persistencia de datos, lo cual es esencial para proyectos de desarrollo de software y despliegues en entornos productivos.





