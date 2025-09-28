# Seguridad en el control de versiones
## Archivos excluidos

1. **Contraseñas y configuraciones privadas (`.env`, `*.env`, `config.local.*`, `*.secret.*`)**  
   - Estos archivos contienen credenciales, claves API, configuraciones sensibles o datos específicos de un entorno local.  
   - Incluirlos en el repositorio podría exponer información crítica a terceros no autorizados.  
   - En su lugar, se recomienda usar gestores de secretos o variables de entorno.  

2. **Logs y archivos temporales (`*.log`, `*.tmp`, `*.swp`)**  
   - Son generados automáticamente durante la ejecución del software o por editores de texto.  
   - No tienen relevancia para el código fuente y solo generan ruido en el control de versiones.  

3. **Binarios y compilados (`*.exe`, `*.dll`, `*.so`, `*.o`, `*.a`, `*.class`)**  
   - Se producen como resultado de la compilación y no deben versionarse.  
   - Mantenerlos fuera del repositorio garantiza que cada desarrollador genere su propia versión a partir del código fuente.  

4. **Directorios de build/dist (`dist/`, `build/`, `out/`)**  
   - Contienen artefactos generados automáticamente durante el proceso de compilación o empaquetado.  
   - No deben subirse, ya que se pueden regenerar en cualquier entorno de desarrollo o integración continua.  
