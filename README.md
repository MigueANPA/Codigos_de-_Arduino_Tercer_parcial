# Codigos_de-_Arduino_Tetcer_parcial
# Código 1: Control de un display de 7 segmentos con números aleatorios

Descripción: Este programa gestiona un display de 7 segmentos conectado a un microcontrolador como Arduino. Genera números aleatorios entre 1 y 6, los cuales se visualizan en el display. Un pulsador permite pausar o reanudar esta generación.

Definiciones iniciales: El array numero almacena las configuraciones de los segmentos para los números del 0 al 9. Un pulsador en el pin 2 controla la pausa y reanudación.

Configuración inicial: Se configuran los pines 3 al 10 como salidas para el display y el pin del pulsador como entrada.

Lógica principal: El estado del pulsador alterna entre pausar y reanudar. Cuando está activo, se genera un número aleatorio cada 50 ms; al estar detenido, se mantiene el último número mostrado.

Control del display: El array numero define qué segmentos se encienden según el número.

Aplicaciones:

Simulación de dados electrónicos.

Introducción a conceptos básicos de electrónica digital.


# Código 2: Control de LEDs con un joystick analógico

Descripción: Este programa permite controlar cuatro LEDs (arriba, abajo, izquierda y derecha) y un LED adicional, dependiendo de la posición y pulsación del joystick.

Definiciones iniciales: Se asignan pines para los LEDs y las conexiones del joystick (ejes X, Y y botón).

Configuración inicial: Los pines de los LEDs se configuran como salidas y el botón con un pull-up interno.

Lógica principal : Los valores de los ejes X e Y determinan cuál LED se enciende, mientras que el botón controla el LED adicional.

Monitorización: Los valores de los ejes y el estado del botón se imprimen en el monitor serial.

Aplicaciones:

Interfaces para videojuegos o robots.

Aprendizaje sobre sensores analógicos.

# Código 3: Teclado matricial para ingresar contraseñas

Descripción: Este programa utiliza un teclado matricial de 4x4 para validar una contraseña ingresada contra una clave maestra predefinida.

Definiciones iniciales: Se configuran las teclas del teclado y la clave maestra.

Configuración inicial: Los LEDs para indicar el resultado de la validación se configuran como salidas.

Lógica principal: Captura y compara la contraseña ingresada con la clave maestra. Si es correcta, enciende un LED verde; si no, uno rojo, ambos durante 2 segundos.

Aplicaciones:

Sistemas básicos de acceso por contraseña.

Ejemplo práctico de uso de teclados matriciales.

# Código 4: Control de un LED RGB con botones

Descripción: Este programa controla un LED RGB mediante tres botones, cada uno asociado a un color primario (rojo, verde y azul).

Definiciones iniciales: Se asignan pines a los colores del LED y a los botones.

Configuración inicial: Los pines del LED y los botones se configuran como salidas y entradas, respectivamente.

Lógica principal: Los botones encienden el color correspondiente del LED RGB usando analogWrite para regular la intensidad.

Aplicaciones:

Introducción al uso de LEDs RGB.

Control básico de iluminación.

# Código 5: Sistema con sensor ultrasónico y servomotor

Descripción: Este programa mide la distancia con un sensor ultrasónico y controla un servomotor para simular la apertura de una puerta, indicando el estado mediante LEDs.

Definiciones iniciales: Se asignan pines para el sensor, LEDs y el servomotor.

Configuración inicial: El sistema comienza con la puerta cerrada y un LED rojo encendido.

Lógica principal: Si un objeto está a menos de 5 cm, el LED verde se enciende, el servomotor abre la puerta, espera 3 segundos y luego la cierra.

Aplicaciones:

Simulación de puertas automáticas.

Sistemas de acceso sin contacto.
![Imagen de WhatsApp 2024-12-09 a las 19 33 51_9368597b](https://github.com/user-attachments/assets/4a1b206a-086a-47ba-90ed-fc9c7fff3c31)



# Código 6: Control de una puerta con servomotor

Descripción: Este programa controla un servomotor que abre y cierra una puerta, indicando el estado mediante LEDs.

Definiciones iniciales: Se configura el servomotor y los LEDs en pines específicos.

Configuración inicial: El servomotor se inicializa en la posición de cerrado.

Lógica principal: Las funciones AbrirPuerta y CerrarPuerta controlan el movimiento gradual del servomotor y el estado de los LEDs.

Aplicaciones:

Simulación de sistemas de acceso controlado.

Demostración práctica del control de servomotores.
