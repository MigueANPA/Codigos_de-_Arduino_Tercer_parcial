# Codigos_de-_Arduino_Tetcer_parcial
Código 1: Control de un display de 7 segmentos con números aleatorios
Descripción: Este programa gestiona un display de 7 segmentos conectado a un microcontrolador como Arduino. Genera números aleatorios entre 1 y 6, los cuales se visualizan en el display. Un pulsador permite pausar o reanudar esta generación.
Funcionamiento:

Definiciones iniciales: El array numero almacena las configuraciones de los segmentos para los números del 0 al 9. Un pulsador en el pin 2 controla la pausa y reanudación.
Configuración inicial (setup): Se configuran los pines 3 al 10 como salidas para el display y el pin del pulsador como entrada.
Lógica principal (loop): El estado del pulsador alterna entre pausar y reanudar. Cuando está activo, se genera un número aleatorio cada 50 ms; al estar detenido, se mantiene el último número mostrado.
Control del display: El array numero define qué segmentos se encienden según el número.
Aplicaciones:
Simulación de dados electrónicos.
Introducción a conceptos básicos de electrónica digital.
