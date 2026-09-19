# Tres ideas de proyecto

> Instrucción: sustituye lo que está entre corchetes y borra las líneas que empiezan con
> "Instrucción:". Las tres ideas son tuyas, no las de tu equipo. En la siguiente sesión el
> equipo decidirá con cuál se queda.

**Autor:** Michel Grande Montalvo
**Fecha:** 18/09/26 

---

## Criterios de viabilidad

Una idea es viable para esta materia si cumple los cuatro criterios:

1. Atiende un **problema concreto de mi entorno** (mi casa, la IBERO, mi colonia, mi municipio), no un tema general.
2. Tiene una **parte física fabricable** con impresión 3D, corte láser o router CNC.
3. Usa **al menos un sensor o un actuador** controlado por un microcontrolador pequeño.
4. Lo puede construir un **equipo de principiantes en unas ocho sesiones**, con materiales accesibles.

---

## Idea 1: Sistema para detectar lugares de estacionamiento disponibles

**Problema.** Cuando hay varios coches o vehiculosbusacndo espacio en el esatcionamiento, no siempre es posible saber rápidamente cuales están disponibles, esto puede provocar que una persona tenga que busacr por un buen tiempo lugares disponibles hasta encontrar uno disaponible.

**A quién le pasa.** En general yo veo a los estudiantes y profesroes de la universidad buscando cupo en el estacionamiento, pero también afecta al personal de IBERO

**Dónde lo he visto.** En el entorno de la universidad, al llegar a pie y veo como siempre hay criculación de vehiculos y como casi siempre están dando vueltas buscando estacionamiento.

**Cómo funcionaría.**
- Qué mide o detecta (sensor): Un sensor ultrasónico detectaría la distancia entre el sensor y el objeto colocado en el espacio de estacionamiento para determinar si está ocupado.
- Qué hace con eso (actuador, aviso, pantalla): Un microcontrolador procesaría la información y encendería un LED verde si el espacio está disponible o un LED rojo si está ocupado. También podría utilizarse una pequeña pantalla para mostrar la cantidad de espacios disponibles.
- Qué pieza habría que fabricar: Una maqueta de un pequeño estacionamiento, con espacios delimitados y soportes para colocar los sensores y los indicadores.

---

## Idea 2: Sistema para saber si un salón está ocupado

**Problema.** En algunos momentos puede ser difícil saber si un salón está siendo utilizado o si se encuentra vacío, especialmente cuando no se tiene la información o el horario de dicho salón, así mismo, cuando hay horas libres y aun se encuentre con estudiantes dentro, lo marque como disponible para que los estudiantes que tengan trabajos pendientes puedan entrar y trabajar ahí(olvidandonos de las salas de computo libre).

**A quién le pasa.** En su mayoria a los estudiantes y a trabajadores del área de limpieza de la IBERO.

**Dónde lo he visto.** En el contexto de las clases en la IBERO, donde los salones pueden estar ocupados durante diferentes horarios y es necesario consultar el horario o acercarse al salón para saber si está siendo utilizado.

**Cómo funcionaría.**
- Qué mide o detecta (sensor): Un sensor de movimiento, como un PIR, detectaría la presencia de personas dentro del salón.
- Qué hace con eso (actuador, aviso, pantalla): El microcontrolador procesaría la señal del sensor y mostraría mediante un LED o una pantalla si el salón está ocupado o disponible.
- Qué pieza habría que fabricar: Una pequeña maqueta de un salón o un módulo para colocar el sensor en la entrada y representar el funcionamiento del sistema.

---

## Idea 3: Sistema para monitorear temperatura y humedad de un salón

**Problema.** La temperatura y la humedad de un salón pueden cambiar durante el día dependiendo de la cantidad de personas, el clima y la ventilación. Sin una medición, solamente se puede saber cómo se siente el ambiente de manera subjetiva.

**A quién le pasa.** A estudiantes y profesores que permanecen durante varias horas dentro de los salones de la IBERO.

**Dónde lo he visto.** En los salones durante las clases, especialmente cuando cambia la cantidad de personas dentro del salón o cuando las condiciones del exterior hacen que el salón se sienta más caliente o húmedo.

**Cómo funcionaría.**
- Qué mide o detecta (sensor): Un sensor de temperatura y humedad, como el DHT11, mediría las condiciones ambientales del salón.
- Qué hace con eso (actuador, aviso, pantalla): El microcontrolador mostraría los valores en una pantalla pequeña y podría activar un LED o un buzzer cuando la temperatura o humedad alcancen o superen(dependiendo lo que se elija) un límite establecido.
- Qué pieza habría que fabricar: Una pequeña carcasa para proteger y colocar el sensor y la pantalla que podría hacerse con una impresora 3D.

---

## Tabla de viabilidad

> Instrucción: escribe Sí, No o Parcial en cada celda. Una idea con un "No" no está
> descalificada: lo que se evalúa es que reconozcas el problema, no que las tres ideas
> salgan perfectas.

| Criterio | Idea 1 | Idea 2 | Idea 3 |
|---|---|---|---|
| Problema concreto de mi entorno | Sí | Sí | Sí |
| Parte física fabricable | Sí | Sí | Sí |
| Sensor o actuador | Sí | Sí | Sí |
| Construible en ocho sesiones por principiantes | Sí | Sí | Sí |
| Qué tan seguro estoy de lo anterior (alto / medio / bajo) | Medio | Medio | Medio |

## Mi elección

**Idea elegida:** Sistema para saber si un salón está ocupado.

**Por qué.** Elegí esta idea porque parte de una situación que he observado y vivido dentro de la IBERO y tiene una utilidad directa para los estudiantes. El proyecto puede realizarse a una escala pequeña utilizando un sensor de movimiento, un microcontrolador y un indicador visual, por lo que creo que es posible construir un prototipo durante las clases. Además, la propuesta podría tener dos usos, ayudar a los estudiantes a identificar espacios disponibles y facilitar al personal de limpieza saber si un salón está vacío.

**Qué todavía no sé.** Todavía necesito comprobar si un sensor PIR es suficiente para determinar correctamente si un salón está ocupado, ya que una persona que permanezca quieta podría dejar de generar movimiento. También necesito investigar cuánto tiempo debería pasar sin detectar movimiento para considerar un salón como disponible y cómo evitar que el sistema marque como vacío un salón en el que todavía haya personas.

---

## Declaración de uso de IA

- **Herramienta utilizada:** ChatGPT — GPT-5.6 Luna.
- **Qué le pedí:** Ayuda para organizar y redactar la propuesta de un sistema que permita detectar si un salón de la IBERO está ocupado, tomando como base el problema que planteé.
- **Qué modifiqué o rechacé de su respuesta, y por qué:** Modifiqué la descripción del problema para enfocarla en la situación específica que he observado en la IBERO: que un salón puede aparecer libre según el horario y aun así estar siendo utilizado por estudiantes. También limité que el proyecto se enfocara en las salas de cómputo del IDIT y limité la propuesta a un prototipo que pueda ser realizado por principiantes.
