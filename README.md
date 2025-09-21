# Simulador de Planificación de Procesos

Este proyecto es un programa hecho en **Java con Swing** que sirve para simular algoritmos de planificación de procesos.  
La idea es poder agregar procesos, elegir un algoritmo (como FCFS, SJF, RR, etc.) y ver cómo se ejecutan y cuáles son sus resultados.

---

## Interfaz del programa

La ventana está dividida en varias partes:

### 1. Controles de simulación
Arriba están las opciones principales:
- Se puede escoger el **algoritmo** a usar.  
- El campo de **quantum** solo se usa si elegimos Round Robin.  
- Hay un botón para **iniciar la simulación** y otro para **reiniciar**.  
- También muestra cuál proceso se está ejecutando y el tiempo actual de la simulación.  

---

### 2. Formulario para agregar procesos
Aquí se escriben los datos de cada proceso:
- **PID:** Identificador.  
- **Nombre:** El nombre del proceso.  
- **Llegada:** El tiempo en que entra.  
- **Duración:** Cuánto tarda en ejecutarse.  
- **Prioridad:** Nivel de prioridad.  

Con el botón **Agregar Proceso**, se manda a la tabla de la izquierda.

---

### 3. Tabla de procesos (izquierda)
Muestra todos los procesos que agregamos. Cada uno aparece con:
- PID, nombre, estado, duración, tiempo restante y el progreso con una barrita.

---

### 4. Cola de listos (centro)
Aquí se ven los procesos que están en estado **READY**.  
Abajo muestra cuántos procesos hay en la cola o si está vacía.

---

### 5. Resultados (derecha)
Cuando la simulación termina, se llenan los resultados:
- **AT**: tiempo de llegada.  
- **BT**: duración.  
- **CT**: tiempo de finalización.  
- **TAT**: tiempo de retorno.  
- **WT**: tiempo de espera.  

---

### 6. Consola de mensajes
En la parte de abajo salen mensajes como “proceso agregado” o cambios de estado.

---

## Cómo usarlo
1. Ejecutar el programa en Eclipse (o cualquier IDE de Java).  
2. Agregar procesos con el formulario.  
3. Elegir un algoritmo y darle en **Iniciar Simulación**.  
4. Ver cómo cambian las tablas y los resultados.  
5. Si quieres empezar de nuevo, usar el botón de **Reiniciar Procesos**.  

---

## Nota
- El quantum solo funciona si se usa **Round Robin**.  
- Los procesos siguen el orden del algoritmo que se escoja.  
