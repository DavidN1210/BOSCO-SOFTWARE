# Seguridad en el control de versiones
## Archivos excluidos

1. **Contraseñas y configuraciones privadas (`.env`, `*.env`, `config.local.*`, `*.secret.*`)**
   
   Estos archivos contienen credenciales, claves API, configuraciones sensibles o datos específicos de un entorno local y incluirlos en el           repositorio puede exponer información importante a terceros no autorizados.  
   En su lugar, se recomienda usar gestores de secretos o variables de entorno.  

2. **Logs y archivos temporales (`*.log`, `*.tmp`, `*.swp`)**  

   Son generados automáticamente durante la ejecución del software o por editores de texto y no tienen relevancia para el código fuente y solo       generan problemas en el control de versiones.  

3. **Binarios y compilados (`*.exe`, `*.dll`, `*.so`, `*.o`, `*.a`, `*.class`)**
   
   Se producen como resultado de la compilación y no deben versionarse, por lo que mantenerlos fuera del repositorio garantiza que cada              desarrollador genere su propia versión a partir del código fuente.  

4. **Directorios de build/dist (`dist/`, `build/`, `out/`)**

   Contienen artefactos generados automáticamente durante el proceso de compilación o empaquetado. Estos no deben subirse, ya que se pueden          regenerar en cualquier entorno de desarrollo o integración continua.

## Prácticas de seguridad

