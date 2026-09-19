# Investigación: ¿esto ya existe? ¿quién lo dice?

> Instrucción: sustituye lo que está entre corchetes y borra las líneas que empiezan con
> "Instrucción:". Todos los enlaces deben abrir. Un enlace roto o inventado anula el
> criterio correspondiente.

**Autor:** Michel Grande Montalvo
**Fecha:** 19/09/26
**Ideas analizadas:** ver [[ideas-proyecto]] o [ideas-proyecto.md](ideas-proyecto.md)

---

## Parte 1. Un ejemplo que ya existe, por cada idea

### Idea 1: Sistema para saber si un salón está ocupado

- **Qué encontré:** Encontré un proyecto llamado Smart Occupancy Based Energy Optimization System, desarrollado con un ESP32 para detectar la ocupación de un salón mediante sensores infrarrojos y un sensor PIR.
- **Enlace:** https://github.com/Ravisankar-S/Occupancy-Based-Energy-Optimization
- **Qué hace:** El proyecto de GitHub utiliza un ESP32, dos sensores infrarrojos para detectar entradas y salidas y un sensor PIR para detectar movimiento. La información se utiliza para mantener un registro de la ocupación y controlar diferentes niveles de iluminación.
- **Por qué no resuelve mi caso:** Estos proyectos tienen un alcance mucho mayor al que necesito para esta materia. Algunos cuentan personas, controlan iluminación, utilizan aplicaciones o almacenan información. Mi propuesta busca comenzar con algo más sencillo: detectar si un salón está siendo utilizado y mostrar claramente si se encuentra ocupado o disponible. Mi objetivo es crear un sistema que funcione sin tener que depender de algo tan complejo.

### Idea 2: Sistema para detectar lugares de estacionamiento disponibles

- **Qué encontré:** Encontré un proyecto llamado Car Parking Simulator, realizado con Arduino, sensores ultrasónicos, una pantalla LCD y LEDs RGB. El proyecto simula un estacionamiento y detecta si los espacios están ocupados.
- **Enlace:** https://projecthub.arduino.cc/bruno_opaiva/car-parking-simulator-522e53
- **Qué hace:** Utiliza sensores ultrasónicos para detectar la distancia y determinar si un lugar de estacionamiento está ocupado. También utiliza LEDs para indicar el estado de los espacios y una pantalla LCD para mostrar información.
- **Por qué no resuelve mi caso:** Es un proyecto de simulación y no está diseñado especificamente para los estacionamientos de la IBERO. Mi propuesta estaría enfocada en detectar la disponibilidad de espacios en un contexto universitario y podria comenzar con una maqueta pequeña para comprobar el funcionamiento.

### Idea 3: Sistema para monitorear temperatura y humedad de un salón

- **Qué encontré:** Encontré un proyecto llamado Temperature and Humidity Monitor Using Whatsapp and ESP32, realizado con un ESP32 y un sensor DHT11.
- **Enlace:** (https://projecthub.arduino.cc/sonutest23/temperature-and-humidity-monitor-using-whatsapp-and-esp32-15e844)
- **Qué hace:** El sistema mide temperatura y humedad mediante un sensor DHT11 conectado a un ESP32 y utiliza conexión Wi-Fi para enviar la información mediante WhatsApp.
- **Por qué no resuelve mi caso:** El proyecto está pensado principalmente para monitorear condiciones ambientales y enviar información mediante internet. Mi propuesta estaría enfocada específicamente en las condiciones de los salones de la IBERO y tendría como objetivo obtener información sencilla sobre el ambiente del espacio. Además no necesitaría comenzar utilizando WhatsApp ni una app externa.

---

## Parte 2. Fuentes de la idea que elegí

### Fuente 1

| Campo | Contenido |
|---|---|
| Autor u organización | Ravisankar S.  |
| Título | Smart Occupancy Based Energy Optimization System |
| Año | 2026 |
| Enlace | https://github.com/Ravisankar-S/Occupancy-Based-Energy-Optimization |
| Tipo | Repositorio / proyecto técnico |
| Por qué le creo | El repositorio muestra directamente el código, los componentes utilizados, la arquitectura del sistema y la forma en que los sensores participan en la detección de ocupación. Además, el proyecto puede ser revisado directamente en el código en lugar de depender solamente de una descripción. |
| Qué dato me dio | El sistema utiliza un ESP32, dos sensores infrarrojos y un sensor PIR. Los sensores infrarrojos se utilizan para detectar la entrada y salida de personas, mientras que el PIR sirve para detectar movimiento y presencia dentro del salón. |

### Fuente 2

| Campo | Contenido |
|---|---|
| Autor u organización | Prakash Karkee |
| Título | Smart Classroom |
| Año | 2025 |
| Enlace | https://github.com/prakashkarkee/smartclass|
| Tipo | Repositorio / proyecto universitario |
| Por qué le creo | El proyecto está publicado en GitHub y señala que fue desarrollado durante un programa de sistemas embebidos de la University of Oulu. El repositorio incluye la descripción del proyecto, los componentes utilizados y el código necesario para su funcionamiento. |
| Qué dato me dio | El proyecto utiliza un ESP32 y diferentes sensores para monitorear un salón inteligente. Entre ellos utiliza un sensor PIR para detectar movimiento, además de sensores para temperatura, humedad, iluminación y sonido. Esto demuestra que un ESP32 puede utilizarse como controlador para recopilar diferentes tipos de información dentro de un salón.|

---

## Parte 3. Qué haría distinto

Mi propuesta estaría enfocada específicamente en los salones de IBERO y no en un sistema completo de automatización del aula.
Buscaría que fuera un proyecto sencillo y de bajo costo, utilizando un sensor PIR, un microcontrolador y una señal visual para indicar si el salón está ocupado o libre.
El dispositivo podría ponerse en la entrada del salón dentro de una pequeña carcasa fabricada en 3D.
Además, se buscaría que el sistema pudiera considerar un tiempo determinado sin movimiento antes de marcar el salón como disponible.

## Parte 4. Qué me falta averiguar

- [ ] ¿Cuánto tiempo sin detectar movimiento debería pasar para considerar que el salón está disponible?
- [ ] ¿El sensor PIR será suficiente para detectar correctamente a una persona que permanezca sentada durante varios minutos?
- [ ] ¿Qué tan bien funciona el sensor en un salón real de IBERO y dónde sería la mejor ubicación para colocarlo?

---

## Declaración de uso de IA

- **Herramienta utilizada:** ChatGPT — GPT-5.6 Luna
- **Qué le pedí:** Ayuda para investigar proyectos similares a mis tres ideas y organizar la información de las fuentes encontradas.
- **Qué modifiqué o rechacé de su respuesta, y por qué:** Modifiqué las propuestas para enfocarlas en el contexto de IBERO y reduje funciones innecesarias y compeljas para que el proyecto sea viable para un estudiante de primer semestre(osea yo). También decidí utilizar solamente dos fuentes para la investigación y mantener como duda técnica el funcionamiento del sensor PIR cuando una persona permanece quieta.
