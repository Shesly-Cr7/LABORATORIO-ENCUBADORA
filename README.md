# LABORATORIO-ENCUBADORA

LABORATORIO-ENCUBADORA
Integrantes Shesly Colorado - 5600756

Santiago Mora - 56

Daniel Herrera - 56

# INTRODUCCIÓN

Las incubadoras neonatales son dispositivos biomédicos fundamentales en las unidades de cuidado intensivo neonatal, diseñados para proporcionar un ambiente controlado que simule las condiciones del vientre materno. Estos sistemas permiten regular variables críticas como la temperatura, la humedad y la ventilación, con el objetivo de garantizar la supervivencia y el desarrollo adecuado de los recién nacidos, especialmente aquellos prematuros o con bajo peso al nacer.

Uno de los factores más importantes en este tipo de sistemas es el control térmico. Los neonatos, particularmente los prematuros, presentan una limitada capacidad de termorregulación debido a su baja cantidad de grasa subcutánea y a la inmadurez de su sistema nervioso, lo que los hace altamente vulnerables a cambios de temperatura. Por esta razón, las incubadoras deben mantener un rango térmico controlado entre aproximadamente 36.5 °C y 37.5 °C, considerado óptimo para evitar complicaciones como hipotermia o hipertermia.

El presente proyecto aborda el diseño e implementación de un sistema de monitoreo de temperatura para una incubadora neonatal a escala, utilizando sensores electrónicos y plataformas de adquisición de datos. Este sistema permite medir, visualizar y analizar la temperatura en tiempo real, integrando herramientas de instrumentación biomédica como microcontroladores y software de procesamiento de señales.

Desde el punto de vista de la instrumentación biomédica, este desarrollo permite aplicar conceptos de adquisición de señales, sensores, procesamiento de datos y visualización, los cuales son esenciales en el diseño de dispositivos médicos. Además, contribuye a comprender la importancia del control preciso de variables fisiológicas en aplicaciones clínicas.

# OBJETIVOS

## Objetivo General
Reconocer la importancia de las incubadoras neonatales en la salud del neonato.

## Objetivos Específicos 
• Identificar las partes principales que componen una incubadora neonatal. 
• Desarrollar un sistema que emule el modo de operación de una incubadora neonatal. 
• Evaluar cómo impacta el control de variables como temperatura, humedad y flujo de aire en la salud del neonato.

# MARCO TEORICO

## 3.1 Incubadora Neonatal

Una incubadora neonatal es un dispositivo médico que proporciona un ambiente controlado de temperatura, humedad y aislamiento para recién nacidos, especialmente prematuros. Su función principal es mantener condiciones térmicas estables y proteger al neonato de factores externos que puedan comprometer su salud .

Estas incubadoras funcionan mediante sistemas de calefacción por convección, donde el aire es calentado y distribuido de manera uniforme dentro de la cámara, reduciendo la pérdida de calor del neonato .

## 3.2 Importancia del Control de Temperatura

El control de temperatura es crítico en neonatología, ya que los recién nacidos no pueden regular eficientemente su temperatura corporal. Un entorno térmico inadecuado puede generar aumento en el consumo de oxígeno, alteraciones metabólicas y riesgo de mortalidad. Por ello, se recomienda mantener la temperatura corporal del neonato entre 36.5 °C y 37.5 °C .

El concepto de ambiente térmico neutro se refiere a las condiciones en las cuales el neonato mantiene su temperatura corporal con un gasto mínimo de energía, lo cual es esencial para su desarrollo adecuado .

## 3.3 Sensores de Temperatura LM35

El LM35 es un sensor de temperatura analógico cuya salida es proporcional a la temperatura en grados Celsius, con una relación de 10 mV/°C. Este tipo de sensor permite una medición directa mediante conversión analógica-digital en el microcontrolador.

### DHT22

El DHT22 es un sensor digital que mide temperatura y humedad relativa, entregando los datos mediante una señal digital procesada internamente. Aunque es más preciso que el DHT11, presenta una menor velocidad de muestreo.

## 3.4 Conversión Analógica y Digital

Los sensores pueden clasificarse según el tipo de señal que generan:

Sensores analógicos (LM35): entregan un voltaje continuo proporcional a la variable medida. Sensores digitales (DHT22): entregan datos procesados en formato digital.

El ESP32 incorpora un convertidor analógico-digital (ADC) que permite transformar señales analógicas en valores digitales para su procesamiento.

## 3.5 Sistema de Monitoreo

El sistema desarrollado en este proyecto sigue una arquitectura básica de instrumentación biomédica:

Sensor → Adquisición (ESP32) → Procesamiento → Visualización (OLED / MATLAB)

Este flujo permite medir, analizar y representar la temperatura en tiempo real, facilitando la toma de decisiones en sistemas biomédicos.

# Materiales y Componentes

## 4.1 Hardware

ESP32 Sensor (DHT22 o LM35) OLED Circuito de fuente

## 4.2 Software

Arduino IDE MATLAB

# SEGURIDAD

Durante el desarrollo del proyecto se deben tener en cuenta las siguientes medidas de seguridad:

Verificar los niveles de voltaje antes de energizar el circuito. No exceder los 3.3 V en los pines del ESP32. Evitar cortocircuitos en la protoboard. Manipular correctamente los equipos electrónicos. Mantener ordenado el espacio de trabajo.

Estas recomendaciones son fundamentales para prevenir daños en los dispositivos y garantizar un desarrollo seguro de la práctica .

# Diseño del Sistema

Parte estructural: 

## 6.1 Sistema de fuente 
Sensor → ESP32 → OLED / MATLAB 
## 6.2 Distema de temperaturaa y peso 
Conexión del sensor Conexión de la OLED 
## 6.3 Funcionamiento 
Cómo se mide la temperatura 
Cómo se procesa 
Cómo se visualiza

# Implementación 

## 7.1 Código Arduino Lectura del sensor Envío serial Visualización OLED

## 7.2 Código MATLAB Lectura serial Gráfica en tiempo real

# Resultados

Gráficas de temperatura Comportamiento del sistema Pruebas realizadas

# Análisis de Resultados
¿La temperatura es estable? ¿Hay ruido en la señal? ¿Qué tan preciso es el sensor? Comparación entre sensores (LM35 vs DHT22)

# Costos 
Lista de componentes con precio Costo total Comparación con incubadoras reales

# Limitaciones del Sistema

No es sistema real médico Falta control automático No mide otras variables (flujo, peso, etc.)

# Conclusiones

Qué aprendiste Qué funcionó Qué mejorarías

# Preguntas de Discusión
• Pregunta 1: ¿Qué otras variables (y por qué) además de las aquí mencionadas son críticas en el monitoreo neonatal?

• Pregunta 2: ¿Qué haría falta para convertir el sistema desarrollado en una incubadora neonatal real?

• Pregunta 3: ¿Qué semejanzas hay entre una incubadora neonatal y una servo-cuna?

# Bibliografía
1. 
