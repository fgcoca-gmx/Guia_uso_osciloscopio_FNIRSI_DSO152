El osciloscopio FNIRSI DSO152 es un mini osciloscopio digital portátil de un canal con un ancho de banda de 200 kHz y una tasa de muestreo de 2.5 MS/s. Se controla mediante una rueda multifunción (joystick) y botones físicos dedicados (AUTO, RUN/STOP, MODE), permitiendo visualizar ondas eléctricas de forma rápida y sencilla.

## <FONT COLOR=#007575>**Controles y Partes del Dispositivo**</font>
* **Pantalla TFT:** Muestra la forma de onda, el voltaje por división, la base de tiempo y el estado del disparador.
* **Rueda de navegación (Joystick superior):** Permite mover el cursor, cambiar parámetros en pantalla y ajustar valores al girar o presionar.
* **Botón AUTO:** Ajusta automáticamente la escala vertical y horizontal para estabilizar la señal en pantalla.
* **Botón RUN/STOP:** Congela o reanuda la lectura de la onda (funciona como una captura de pantalla en tiempo real).
* **Botón MODE:** Cambia los modos de disparo (Auto, Normal, Single).
* **Puerto USB Tipo C:** Sirve para cargar la batería interna de 1000 mAh.
* **Conector de entrada de señal:** Donde se conecta la sonda (punta de prueba).

La pantalla muestra:

![Pantalla](../img/osc/pantalla_sen.png){.center-img100}

!!! Note "Cyc"
    En la pantalla se observa la abreviatura Cyc que proviene del inglés Cycle (Ciclo) o Cycle Period. Significa que la onda tarda exactamente 0.100 milisegundos (ms), lo que equivale a 100 microsegundos (μs) que es justo el Time/div fijado para un cuadro en horizontal.

El FNIRSI DSO152 calcula automáticamente los datos de la señal medida.

## <FONT COLOR=#007575>**Ejemplos**</font>
En la imagen siguiente vemos una señal cuadrada:

![Cuadrada](../img/osc/cuadrada.png){.center-img75}

En la imagen siguiente vemos una señal triangular:

![Triangular](../img/osc/triangular.png){.center-img75}

En la imagen siguiente vemos una señal diente de sierra de rampa ascendente (Sawtooth):

![Diente de sierra ascendente](../img/osc/diente_asc.png){.center-img75}

En la imagen siguiente vemos una señal diente de sierra de rampa descendente (ReSawtooth):

![Diente de sierra descendente](../img/osc/diente_des.png){.center-img75}

## <FONT COLOR=#007575>**Procesos**</font>
El terminal de la sonda tiene una punta o pinza de medida y una pinza de masa. La pinza de masa debe conectarse siempre al GND del circuito y no debes dejarla nunca desconectada.

Si dispones de una sonda ×10 puedes conectarla a la salida de calibración (onda cuadrada de 1 kHz). Selecciona ×10 en la sonda y en el osciloscopio y ajusta el pequeño condensador de compensación hasta obtener una onda cuadrada con flancos rectos.

Recuerda que el acoplamiento AC/DC es habitual tenerlo en DC para que muestre continua y alterna y que en la posición AC elimina la componente continua, lo que resulta muy útil para señales de audio, señales pequeñas superpuestas a un nivel DC, rizados, etc.

Para medir una fuente de alimentación:

* Selecciona DC y observa la tensión continua y el rizado (Ripple).
* Para apreciar mejor el rizado selecciona AC y reduce los V/div.

Aunque es una excelente herramienta para iniciarse, conviene conocer sus límites:

* Solo dispone de 1 canal, por lo que no permite comparar dos señales simultáneamente.
* Su ancho de banda de 200 kHz lo hace adecuado para electrónica básica, audio, sensores y microcontroladores, pero insuficiente para señales rápidas como USB, Ethernet o buses digitales de alta velocidad.
* No incorpora funciones avanzadas como decodificación de protocolos, análisis FFT o memoria profunda.

Como conclusión se puede decir que FNIRSI DSO152 es un osciloscopio portátil muy adecuado para aprender los fundamentos del análisis de señales y realizar tareas de diagnóstico en electrónica básica. Su botón AUTO, los modos de disparo y la posibilidad de trabajar con acoplamiento AC/DC permiten obtener resultados útiles con una curva de aprendizaje relativamente corta, siempre respetando sus limitaciones de ancho de banda y tensión de entrada.
