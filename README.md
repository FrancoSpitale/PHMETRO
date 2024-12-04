
Resumen del Proyecto: Medidor de pH
Este documento describe la implementación de un medidor de pH utilizando un microcontrolador PIC, incluyendo el diseño del hardware, acondicionamiento de señal y software. A continuación, se presenta un resumen de las principales secciones:

Introducción
Un medidor de pH mide la concentración de iones hidrógeno en una solución.
El sistema se basa en un electrodo ion-selectivo y un amplificador operacional para procesar la señal antes de enviarla al microcontrolador.
Diseño del Sistema
Hardware:

Electrodo de pH: Produce una señal en milivoltios proporcional al pH de la solución.
Etapa de Acondicionamiento:
Amplificador Operacional: Aumenta la señal débil del electrodo.
Filtro: Elimina ruido eléctrico.
Adaptación de Niveles: Ajusta la señal para el rango aceptado por el ADC del microcontrolador.
Microcontrolador PIC: Realiza la conversión de señales analógicas a digitales y calcula el pH.
Software:

Escrito en lenguaje C.
Maneja:
Configuración de ADC para la lectura analógica.
Conversión de la señal a valores de pH usando fórmulas calibradas.
Interfaz con un display LCD para mostrar el resultado.
Funciones de calibración para asegurar precisión.
Teoría del pH
Definición: El pH es una escala logarítmica para medir la acidez o alcalinidad de una solución.
Rango típico: 0 (muy ácido) a 14 (muy alcalino).
Potencial del electrodo: Cambia aproximadamente 59.16 mV por unidad de pH a 25 °C.
Implementación del Código
Incluye configuraciones específicas para el PIC:
Configuración del ADC para 10 bits.
Cálculos matemáticos para convertir la señal analógica en valores de pH.
Menú de calibración para ajustar las mediciones basadas en soluciones de referencia.
Calibración
Utiliza soluciones buffer estándar (pH 4, pH 7 y pH 10) para ajustar la escala y pendiente del sistema.
Asegura precisión en diferentes rangos de medición.
Resultados
El medidor muestra valores precisos de pH en un display LCD.
Puede ser aplicado en laboratorios, acuarios, procesos industriales y otras áreas que requieran monitoreo de pH.
Conclusión
El proyecto demuestra cómo se puede implementar un medidor de pH funcional usando electrónica analógica y digital básica. Se enfatiza en la importancia de la calibración para obtener resultados precisos.

