# Proyecto Curiosity

El proyecto "Curiosity" consiste en una simulación de las actividades e interacción entre el rover "Curiosity" y su centro de control de misión en la NASA. El proyecto tiene como objetivo desarrollar un sistema que pueda simular los movimientos del rover, analizar la superficie marciana y planificar actividades de exploración.

Este proyecto fue desarrollado en la univerisdad para la asignatura de Estructuras de Datos, donde se ven estructuras lineales —como lo son Listas y Vectores— y estructuras no lineales —como Árboles y Grafos—.

---

## Características

- **Gestión de Comandos**: Se cargan y gestionan comandos de movimiento y datos de puntos de interés desde archivos usando estructuras de datos lineales.
- **Simulación de Movimiento**: Se simula la ejecución de comandos de movimiento y se valida la nueva posición del rover en la superficie marciana.
- **Localización de Elementos**: Se almacenan y ubican puntos de interés (rocas, cráteres, dunas) utilizando una estructura de datos jerárquica (Quadtree) para consultas espaciales eficientes.
- **Creación de Mapas Geográficos**: Se genera una representación basada en grafos de la superficie marciana conectando puntos de interés según un coeficiente de conectividad y distancias euclidianas.
- **Identificación del Camino Más Largo**: Se identifica el camino más largo entre dos puntos de interés dentro del mapa generado, facilitando la planificación de rutas para actividades de exploración.
- **Interfaz Interactiva de Línea de Comandos**: Se interactua con el sistema a través de una interfaz de línea de comandos, permitiendo a los usuarios ejecutar varios comandos y recibir mensajes de éxito/error apropiados.


## Comandos de Ejemplo

- `cargar_comandos <filename>`: Cargar comandos de movimiento desde un archivo.
- `cargar_elementos <filename>`: Cargar datos de puntos de interés desde un archivo.
- `agregar_movimiento <type> <magnitude> <unit>`: Agregar un comando de movimiento a la lista de comandos del rover.
- `agregar_analisis <type> <object> <comment>`: Agregar un comando de análisis a la lista de comandos del rover.
- `agregar_elemento <type> <size> <unit> <x> <y>`: Agregar un nuevo punto de interés al sistema.
- `guardar <type> <filename>`: Guardar los comandos cargados o datos de puntos de interés en un archivo.
- `simular_comandos <x> <y>`: Simular la ejecución de comandos de movimiento comenzando desde las coordenadas dadas.
- `ubicar_elementos`: Ubicar los puntos de interés utilizando una estructura de datos Quadtree.
- `en_cuadrante <x1> <x2> <y1> <y2>`: Recuperar una lista de puntos de interés dentro de un cuadrante geográfico especificado.
- `crear_mapa <connectivity_coefficient>`: Crear una representación del mapa conectando puntos de interés según el coeficiente de conectividad dado.
- `ruta_mas_larga`: Encontrar el camino más largo entre dos puntos de interés dentro del mapa generado.


## Licencia

Este proyecto fue licenciado bajo la [Licencia MIT](LICENSE).
