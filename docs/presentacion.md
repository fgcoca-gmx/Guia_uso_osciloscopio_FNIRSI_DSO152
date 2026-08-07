## <FONT COLOR=#007575>**Partes**</font>

En la imagen se describen las partes del osciloscopio:

![Partes del osciloscopio](../img/osc/partes.png){.center-img100}

## <FONT COLOR=#007575>**Funcionalidad de los botones**</font>
A continuación se describe la funcionalidad básica de los botones.

|Botón|Pulsación|Función|
|:-:|---|---|
|![Botón rueda a la izquierda](../img/osc/B_rueda_izda.png)|Corta |Selección de la función de los parámetros de control |
|![Pulsación del botón rueda](../img/osc/B_rueda_pulsa.png)|Corta |Salir de la calibración automática (página de calibración automática)
 |
|![Pulsación del botón rueda](../img/osc/B_rueda_pulsa.png)|Larga |Acceso a la página de calibración automática |
|![Botón rueda a la derecha](../img/osc/B_rueda_dcha.png)|Corta |Selección de la función de los parámetros de control
 |
|![Botón AUTO](../img/osc/B_auto.png)|Corta |Ajuste automático<br>(las frecuencias inferiores a 45 Hz no se pueden calibrar correctamente)</br> |
|![Botón MODE](../img/osc/B_mode.png)|Corta|Selección entre AUTO, Individual y Normal |
|![Botón MODE](../img/osc/B_mode.png)|Larga|Conmutación por flanco ascendente/descendente
 |
|![Botón arriba](../img/osc/B_up.png)|Corta |Ajuste por adición de parámetros |
|![Botón abajo](../img/osc/B_down.png)|Corta |Ajuste por sustracción de parámetros |
|![Botón RUN](../img/osc/B_run.png)|Corta |Ejecutar/pausar formas de onda (otras páginas)<br>Acceder a la calibración automática (página de calibración automática)</br> |
|![Botón RUN](../img/osc/B_run.png)|Larga |Mostrar/ocultar detalle de parámetros |
|![Botón on/off](../img/osc/B_on_off.png)|Corta |Apagar (OFF)|
|![Botón on/off](../img/osc/B_on_off.png)| Larga|Encender (ON)|

## <FONT COLOR=#007575>**Características**</font>

* Velocidad de muestreo (Sampling rate): 2,5 MS/s
* Sensibilidad vertical: de 10 mV/Div a 10V/Div (Cambios en 1-2-5)
* Ancho de banda (Bandwidth): 200K
* Rango de la base de tiempo (Time base range): de 10 μs/Div a 50s/Div (Cambios en 1-2-5)
* Rango de tensión (Voltage range): X1 :士40 V (Vpp: 80 V) / X10: 士400 V (Vpp: 800 V)
* Método de disparo (Trigger): Auto/Normal/Single
* Método de acoplamiento (Coupling method): AC/DC
* Pantalla: 2,8 pulgadas / PPI:320x240
* Carga USB: 5V/1A
* Capacidad de la bateria: 1000 mAh
* Onda cuadrada de calibración: Frecuencia: 1 K / Ciclo de trabajo: 50 %
* Tamaño: 99 x 68,3 x 19,5 mm
* Peso: 100 g

## <FONT COLOR=#007575>**Pantalla**</font>

![Partes de la pantalla](../img/osc/partes_pantalla.png){.center-img100}

* ① Icono indicador del modo de disparo: "Auto" significa disparo automático, "Single" significa disparo único y "Normal" significa disparo normal.
* ② Icono indicador de la línea de base: este icono indica que la posición actual corresponde a la tensión OV.
* ③ Sensibilidad vertical: se refiere a la tensión representada por una cuadrícula en dirección vertical.
* ④ Icono indicador del modo 1X/10X: debe coincidir con el ajuste del selector 1X/10X situado en el mango de la sonda; si la sonda está en modo 1X, el osciloscopio también debe estar ajustado en modo 1X; el modo 1X mide una tensión de ±40 V, mientras que el modo 10X mide una tensión de ±400 V.
* ⑤ Base de tiempo horizontal, que indica la duración representada por una cuadrícula en dirección horizontal.
* ⑥ Icono indicador de acoplamiento de entrada: "AC" para corriente alterna y "DC" para corriente continua.
* ⑦ Icono del indicador de funcionamiento: RUN significa en funcionamiento y STOP significa en pausa.
* ⑧ Icono del indicador de tensión de disparo
* ⑨ Icono del indicador de flanco de disparo

## <FONT COLOR=#007575>**Actualizar el firmware**</font>
El dispositivo utiliza *USB analog U disk (disco U simulado o virtual)* para actualizar el firmware, y los pasos para la actualización son los siguientes:

1. Mantén presionado el botón OK y, sin soltarlo, enciende el dispositivo para entrar en modo disco virtual ("DSO BOOT") y acceder al modo de actualización mediante memoria USB.
3. Utiliza el cable USB-C para conectar la placa al ordenador. En ese momento, el ordenador mostrará una memoria USB denominada "DSO BOOT".
4. El ordenador reconocerá el aparato como una unidad de almacenamiento virtual o disco USB con el nombre "DSO BOOT".
5. Copia y pega el firmware en la memoria USB montada. Puedes descargar el firmware actual desde [FNIRSI Manuals & Firmware Downloads](https://www.fnirsi.com/pages/manuals-firmwares?srsltid=AfmBOoq_03TCkGA7FVbUbaW_N4RCR3SoXDqvuAfZ5kbLDmSLbRvIBBKM).
6. El proceso de carga comenzará de manera automática; al finalizar, el dispositivo se reiniciará solo con el nuevo sistema operativo funcionando.

!!! Note "USB analog U disk"
    Es una función en la que un dispositivo electrónico actúa ante un ordenador como si fuera una memoria USB convencional, permitiendo transferir archivos de forma interna sin usar un pendrive físico.

Si trabajas con Linux (Ubuntu en mi caso), para actualizar el firmware del osciloscopio FNIRSI DSO152, no necesitas software especial ya que el dispositivo se monta de forma nativa como una unidad de almacenamiento USB ("U disk") en modo de actualización. En la imagen siguiente vemos el resultado del comando ```lsblk``` ejecutado en una terminal.

![Unidad DSO BOOT montada](../img/osc/DSO_BOOT_montada.png){.center-img100}

Al entrar en el modo disco virtual ("DSO BOOT") el osciloscopio muestra la pantalla siguiente:

![Modo actualización de firmware](../img/osc/modo_act_firmw.png){.center-img75}

Que se traduce por:

![Modo actualización de firmware](../img/osc/modo_act_firmwSP.png){.center-img75}

Para salir del modo de actualización:

* **Desconectar USB:** Retira el cable USB-C que conecta el osciloscopio al ordenador para cortar la comunicación de almacenamiento masivo.
* **Forzar apagado o reinicio:** Mantén presionado el botón de encendido (Power) durante unos segundos para apagar la unidad. Si no responde, inserta la punta de un clip metálico, un cable dupont macho o un alfiler en el orificio de reset ubicado en el lateral (cerca del puerto USB-C) para forzar un reinicio físico.
* **Encendido normal:** Vuelve a encender el dispositivo de forma habitual sin presionar el botón OK para que cargue la interfaz normal del osciloscopio.

## <FONT COLOR=#007575>**Precauciones**</font>
* Una vez recibido el dispositivo, utilízalo solo después de haberlo cargado por completo.
* Al utilizar el osciloscopio, presta atención a la selección del conector; el conector del osciloscopio debe coincidir con el de la sonda.
* Al medir tensiones elevadas, está prohibido tocar cualquier pieza metálica del osciloscopio para evitar el riesgo de descarga eléctrica.
* Intenta no realizar pruebas con tensión elevada mientras se está cargando el dispositivo.
* Durante la calibración, es necesario desconectar la sonda BNC o cortocircuitar los polos positivo y negativo de la sonda.
* En la actualización del firmware por USB está prohibido arrastrar archivos que no sean el firmware oficial; de lo contrario, podrías provocar consecuencias irreparables.
* Utiliza una tensión que se encuentre dentro del rango especificado en el manual para la recarga.
