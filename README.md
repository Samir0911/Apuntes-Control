### Samir Romero - 87382
### Miguel Rueda -

# Clase # 1

---

# Apuntes sobre Control de Movimiento

## ¿Qué es el Control de Movimiento?

El **control de movimiento**, también conocido como "robótica", se refiere al uso de sistemas para mover cargas de manera controlada en procesos industriales. ([Fuente](https://www.a-m-c.com/es/vista-general-del-control-de-movimiento/?utm_source=chatgpt.com))

## Aplicaciones del Control de Movimiento

El control de movimiento se utiliza en una variedad de aplicaciones industriales, incluyendo:

- **Impresoras**: Para posicionar con precisión el cabezal de impresión y el papel. (ver Figura 1)
- **Cortadoras**: Para dirigir herramientas de corte en trayectorias específicas. (ver Figura 2)
- **Máquinas dobladoras**: Para controlar el ángulo y la posición en operaciones de doblado de materiales. (ver Figura 3)

## Tipos de Movimientos en el Control de Movimiento

- **Movimiento Lineal**: Desplazamiento en línea recta.
- **Movimiento Rotacional**: Giro alrededor de un eje.
- **Movimiento Combinado**: Integración de movimientos lineales y rotacionales para lograr trayectorias complejas.

## Ejemplo: Impresoras

En las impresoras, el control de movimiento es esencial para:

- **Posicionamiento del Cabezal de Impresión**: Mover el cabezal a lo largo del papel con precisión.
- **Alimentación del Papel**: Controlar el avance del papel para asegurar una impresión uniforme.

## Aplicaciones que Usan Control de Movimiento

| Aplicación           | Descripción                                                                                 |
|----------------------|---------------------------------------------------------------------------------------------|
| **Cortadoras**       | Máquinas que emplean control de movimiento para dirigir herramientas de corte con precisión.|
| **Máquinas Dobladoras** | Equipos que utilizan sistemas de control para realizar dobleces exactos en materiales.    |
| **Máquinas CNC**     | Equipos que realizan operaciones de mecanizado controladas por computadora.                 |

## Evolución del Control de Movimiento

### Antes del Control de Movimiento Moderno

- **Uso de Motores Grandes**: Se empleaban motores de gran tamaño para accionar múltiples mecanismos.
- **Engranajes y Transmisiones Mecánicas**: Complejos sistemas de engranajes transmitían el movimiento desde un único motor a diferentes partes de la máquina.

### Mejoras con el Control de Movimiento

- **Precisión Incrementada**: Los sistemas modernos permiten un control más exacto de posiciones y velocidades.
- **Reducción de Tamaño y Complejidad**: Se utilizan motores más pequeños y sistemas electrónicos, disminuyendo la necesidad de engranajes voluminosos.
- **Flexibilidad Operativa**: Es más sencillo reprogramar y adaptar máquinas para diferentes tareas sin modificaciones mecánicas extensas.

## Espacios para Figuras

A continuación, se sugieren espacios para incluir figuras que complementen los temas tratados:

1. **Figura 1**: Diagrama de una impresora mostrando los componentes controlados por sistemas de movimiento.
   ([Fuente](esquema1.png))
3. **Figura 2**: Imagen comparativa entre una máquina antigua con múltiples engranajes y una moderna con control de movimiento avanzado.
4. **Figura 3**: Esquema de una máquina dobladora que ilustre cómo el control de movimiento influye en el proceso de doblado.

Estas figuras ayudarán a visualizar los conceptos y la evolución en el control de movimiento dentro de diversas aplicaciones industriales.

---

# Clase #2

## Control de Movimiento
El control de movimiento es un aspecto crucial en ingeniería, especialmente en sistemas que requieren mantener condiciones específicas, como temperatura, presión o velocidad.

### Control Cascada
El control cascada es una técnica utilizada en sistemas de control para mejorar la estabilidad y precisión del control. En este método, se utilizan múltiples lazos de control, donde el error de un lazo se utiliza como entrada para otro lazo.

#### Definición
*Control Cascada*: Es un sistema de control que utiliza múltiples lazos de retroalimentación para mejorar la precisión y estabilidad del sistema. Cada lazo se encarga de controlar una variable específica, y el error de un lazo se utiliza como referencia para el siguiente.

#### Ejemplo: Control de Velocidad en un Motor Eléctrico
En este ejemplo, el motor tiene un sensor que mide la velocidad actual y envía esta información al controlador. El controlador compara la velocidad actual con el punto de consigna (velocidad deseada) y ajusta la corriente eléctrica para mantener la velocidad dentro del rango deseado.

1. **Sensor de Velocidad:**: Mide la velocidad actual del motor.
2. **Controlador**: Compara la velocidad actual con el punto de consigna y ajusta la corriente eléctrica.
3. **Elemento Final de Control**:En este caso, un controlador de corriente que ajusta la corriente eléctrica al motor.

**Limitaciones del Control Directo**  
Aunque el control directo es simple y efectivo para muchos procesos, puede tener limitaciones en términos de precisión y estabilidad, especialmente cuando se enfrenta a perturbaciones externas.

---

### Mejora con Control Cascada
En el ejemplo del motor eléctrico, podríamos agregar un segundo lazo que controle la corriente eléctrica que llega al motor. Este lazo actúa como un lazo interno que ajusta la corriente para asegurar que la potencia entregada sea precisa.

#### Esquema con Control Cascada
- **Lazo Externo**: Controla la velocidad del motor comparando la velocidad actual con el punto de consigna.
- **Lazo Interno**: Controla la corriente eléctrica para asegurar que la potencia entregada al motor sea precisa.

---

### Ecuaciones Básicas para Control de Velocidad
Para entender cómo funciona el control de velocidad, podemos considerar la ecuación básica del torque en un motor eléctrico:

   T = k_t × I

   
Donde:
- T* es el torque del motor.
- *k_t* es el coeficiente de torque.
- *I* es la corriente eléctrica.

---

### Tabla Comparativa: Control Directo vs. Control Cascada

| Característica | Control Directo | Control Cascada |
|----------------|-----------------|-----------------|
| Precisión      | Menor           | Mayor           |
| Estabilidad    | Menor           | Mayor           |
| Complejidad    | Menor           | Mayor           |

---

### Espacio para Figura: Esquema de Control de Temperatura


---

### Espacio para Figura: Representación del Control Cascada
*(Aquí puedes insertar una figura que ilustre cómo funciona el control cascada en un sistema).*
