# Programando-Un-Proceso

# Simulador de Planificación de Procesos

Este proyecto es una aplicación en **Java Swing** que simula algoritmos de planificación de procesos (como **FCFS**, **SJF**, **Round Robin**, etc.).  
La interfaz gráfica permite agregar procesos, ejecutar la simulación y visualizar los resultados de manera clara y ordenada.  

---

## 🖼️ Interfaz Gráfica

![Interfaz del Simulador](CapturaSwing.PNG)

La interfaz está dividida en varias secciones:

### 1. Control de Simulación (parte superior)
- **Algoritmo:** Menú desplegable para seleccionar el algoritmo de planificación.  
- **Quantum:** Campo editable que solo se usa en Round Robin.  
- **Botón "Iniciar Simulación":** Comienza la ejecución de los procesos.  
- **Botón "Reiniciar Procesos":** Limpia todos los procesos y tablas.  
- **Proceso en ejecución:** Muestra qué proceso se está ejecutando actualmente.  
- **Tiempo:** Contador del tiempo de simulación.  

---

### 2. Formulario de creación de procesos
Campos para ingresar manualmente la información de cada proceso:
- **PID:** Identificador del proceso.  
- **Nombre:** Nombre del proceso.  
- **Llegada:** Tiempo de llegada (AT).  
- **Duración:** Tiempo de ráfaga o Burst Time (BT).  
- **Prioridad:** Nivel de prioridad (si aplica).  

Luego, con el botón **Agregar Proceso**, el proceso aparece en la tabla de la izquierda.  

---

### 3. Tabla de Procesos (izquierda)
- Muestra todos los procesos creados con sus atributos:  
  - PID  
  - Nombre  
  - Estado  
  - Duración (BT)  
  - Restante (tiempo de ejecución pendiente)  
  - Progreso (barra visual de avance)  

---

### 4. Cola de Procesos Listos (centro)
- Representa los procesos que están en **estado READY**.  
- Incluye columnas con:
  - PID  
  - Nombre  
  - Estado  
  - Llegada (AT)  
  - Restante  
  - Prioridad  
- Abajo indica cuántos procesos hay en la cola.  

---

### 5. Resultados del Algoritmo (derecha)
- Muestra las métricas finales de cada proceso después de la simulación:  
  - **Proceso**  
  - **AT** (Arrival Time)  
  - **BT** (Burst Time)  
  - **CT** (Completion Time)  
  - **TAT** (Turnaround Time)  
  - **WT** (Waiting Time)  

---

### 6. Consola de mensajes (parte inferior)
- Muestra registros de las acciones realizadas, por ejemplo:  
  - Proceso agregado  
  - Estado del sistema  
  - Mensajes de la simulación  

---

## 🚀 Ejecución
1. Compila el proyecto en Eclipse o cualquier IDE de Java.  
2. Ejecuta la clase principal (`Main` o la que contenga el método `main`).  
3. Agrega procesos, selecciona un algoritmo y haz clic en **Iniciar Simulación**.  

---

## 📌 Notas
- El campo **Quantum** solo se activa si el algoritmo elegido es **Round Robin**.  
- Los procesos se ejecutan de acuerdo al algoritmo seleccionado.  
- Puedes reiniciar la simulación en cualquier momento con el botón correspondiente.  
