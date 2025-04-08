# Prueba usando CalBasica

---

## Enunciado de la Práctica: Gestión de Cálculos con Logs y Argumentos

### Título:
**Desarrollo de una calculadora básica con soporte de argumentos y sistema de registro (log)**

### Objetivo:
Crear una aplicación Kotlin basada en consola que implemente operaciones aritméticas básicas utilizando una arquitectura modular y principios de diseño orientados a objetos (POO) y principios SOLID. Además, gestionará argumentos por línea de comandos y mantendrá un registro de las operaciones realizadas en un sistema de logs.

### Requisitos funcionales:

1. **Comportamiento según los argumentos de entrada:**
   - **Sin argumentos:**  
     - Buscar la carpeta `./log`.  
     - Si no existe, crearla y mostrar: `"Ruta ./log creada"`  
     - Si existe y hay archivos, abrir el más reciente (`logYYYYMMDDHHMMSS.txt`) y mostrar su contenido línea por línea.  
     - Si no existen logs, mostrar: `"No existen ficheros de Log"`  

   - **Un argumento:**  
     - Se interpreta como la ruta de los logs.  
     - Mismo comportamiento que el caso anterior pero con la ruta proporcionada.  

   - **Cuatro argumentos:**  
     - El primero: ruta del log.  
     - Segundo y cuarto: números.  
     - Tercero: operador.  
     - Ejecuta el cálculo indicado, muestra el resultado o el error, y lo almacena en un nuevo fichero de log creado con formato `logYYYYMMDDHHMMSS.txt`.  

   - **Cualquier otro número de argumentos:**  
     - Mostrar error y no iniciar el programa.

2. **Cálculos en bucle:**
   - Después del manejo de argumentos, mostrar una pausa.
   - Limpiar pantalla.
   - Lanzar el programa de calculadora en bucle hasta que el usuario indique que no desea seguir.
   - Cada operación realizada se registra en el log actual, incluyendo fecha y hora (con segundos) y el resultado o error.
