# Pendulo_invertido
!(images/Pendulo.jpeg)
Realización de un péndulo invertido para la asignatura de Teoria de control en USC Robótica.

La motivación de este proyecto ha sido crear un chasis de un solo eje con dos ruedas tratando de hacer que mediante un contolador PID no se caiga en ninún momento.
La electrónica de este proyecto está contenida en una PCB diseñada en KiCad y los componentes serán descritos a lo largo de este documento.

# Creación PCB
Primero de todo, hemos creado un prototipo basándonos en modelos realizados por compañeros de años anteriores. La placa contenía las tres huellas de los componentes principales:

- **ESP32:** microcontrolador utilizado para gestionar la información proveniente del acelerómetro, calcular la salida del controlador PID y enviar las órdenes correspondientes a los motores.

- **GY-521:** sensor utilizado para medir la inclinación mediante los tres ángulos de Euler:
  - **Roll**
  - **Pitch**
  - **Yaw**

- **ROB-14450:** Puente-h encargado de regular el voltaje que va hacia los motores
- **Regulador de voltaje, formado por:**
  - **2 condensadores cerámicos de 10uF:** Necesarios para el regulador
  - **LM-7805:** Regula de los ~14V de entrada a 5V para alimetar el microcontrolador
  - **Diodo 1N4743A:** Para no quemar el circuito
  
- **Portapilas x3:** Donde van pilas con una carga de 4.7V
- **2 Motores GA25-370**


