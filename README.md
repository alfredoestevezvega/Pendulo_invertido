# Pendulo_invertido
Realización de un péndulo invertido para la asignatura de Teoria de control en USC Robótica.

La motivación de este proyecto ha sido crear un chasis de un solo eje con dos ruedas tratando de hacer que mediante un contolador PID no se caiga en ninún momento.
La electrónica de este proyecto está contenida en una PCB diseñada en KiCad y los componentes serán descritos a lo largo de este documento.

# Creación PCB
Primero de todo hemos creado un prototipo basándonos en modelos de compañeros anteriores, donde la placa contenia las 3 huellas de los componentes principales:
-Esp32: Este es el microcontrolador utilizado para la gestión de información proveniente del acelerómetro y para calcular la salida del PID y relacionarla con los motores
-Gy-521: Sensor utilizado para medir la inclinación en los 3 ángulos de euler (Roll, pich, yaw).
-Rob
