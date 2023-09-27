# Teoira-de-Colas
 Colas de Prioridad
Universidad Jose Antonio Páez
Métodos Cuantitativos
-Las importaciones y el uso de la cola de prioridad (`PriorityQueue`) están relacionados con la estructura de datos que se utiliza en el código para administrar los procesos en una cola basada en su prioridad. 

-La clase `PriorityQueue` en Java es parte del paquete `java.util` y se utiliza para implementar una cola de prioridad basada en un montículo. Un montículo es una estructura de datos en forma de árbol en la que el elemento principal (raíz) tiene la mayor prioridad o el valor más alto. En este caso, se está utilizando `PriorityQueue` para administrar los procesos en función de sus cuantums o prioridades.

** C O D I G O **
El Codigo realiza una simulación simplificada de la planificación de procesos utilizando una cola de prioridad, con una interfaz gráfica de usuario construida utilizando componentes Java Swing. Modela la ejecución de procesos y muestra su progreso y resultados.

1. La clase `Procesar` extiende `javax.swing.JFrame` y representa la ventana principal de la aplicación.

2. La clase contiene diversas variables de instancia para gestionar el estado de la aplicación, incluyendo contadores, detalles de procesos, una cola de procesos (`colaProcesos`) y el proceso que se está ejecutando actualmente (`procesoEjecutando`).

3. La clase interna `Hilo` es una clase anidada que implementa la interfaz `Runnable`. Esta clase simula la ejecución de procesos en un hilo separado.

4. En el método `run()` de `Hilo`:
   - El hilo entra en un bucle mientras haya procesos en la cola (`colaProcesos`).
   - Se obtiene el próximo proceso a ejecutar de la cola usando el método `poll()`.
   - Si el proceso obtenido no es nulo, comienza la simulación de ejecución del proceso.
   - Se decrementa el tiempo de ráfaga restante del proceso en un bucle hasta que llega a cero.
   - Se actualiza la interfaz de usuario para mostrar el proceso como "Procesando" y se actualiza la barra de progreso.
   - Se incrementa el tiempo de ejecución del proceso (`TiempoProceso`) y se introduce un retraso (`Dormir()`).
   - Después de que el proceso finaliza, se marca como "Terminado" y se registran sus detalles en la tabla de procesos finales (`jTFinal`).
   - Se actualiza la interfaz de usuario con la información de terminación y se elimina el proceso de la cola.

5. El método `Dormir()` introduce un retraso para simular el tiempo de procesamiento.

6. El método `Cargar()` carga los detalles del proceso desde la tabla.

7. El método `Ingresar()` agrega un nuevo proceso a la tabla y lo encola en la cola de prioridad.

8. El método `Informe()` actualiza la tabla de procesos finales y muestra el tiempo de ejecución de cada proceso.

9. El método `Borrar()` elimina los detalles de un proceso finalizado de la tabla de entrada.

10. El método `Barra()` calcula y actualiza el progreso de la barra de progreso.

11. El método `Pintar()` actualiza la interfaz de usuario con el estado actual de la barra de progreso.

12. El método `Iniciar()` oculta los componentes de entrada para evitar cambios durante la ejecución de los procesos.

13. La clase interna `Proceso` representa un proceso con atributos como número, tiempo de ráfaga, tiempo de quantum y tiempo de ráfaga restante. Implementa la interfaz `Comparable` para la comparación de prioridad.

14. El método `main()` inicia la aplicación Swing creando una instancia de la clase `Procesar`.







 Lanzamiento de dardos 


 programación entera 

