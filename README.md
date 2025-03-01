### Andrey Samir Romero Buitrago - 87382
### Miguel Ángel Rueda Santana - 73786

# Clase # 1

---

# Apuntes sobre Control de Movimiento

## ¿Qué es el Control de Movimiento?

El **control de movimiento**, también conocido como "robótica", se refiere al uso de sistemas para mover cargas de manera controlada en procesos industriales. ([Fuente](https://www.a-m-c.com/es/vista-general-del-control-de-movimiento/?utm_source=chatgpt.com))

## Aplicaciones del Control de Movimiento

El control de movimiento se utiliza en una variedad de aplicaciones industriales, incluyendo:

- **Impresoras**: Para posicionar con precisión el cabezal de impresión y el papel. (ver Figura 1)
- **Cortadoras**: Para dirigir herramientas de corte en trayectorias específicas. 
- **Máquinas dobladoras**: Para controlar el ángulo y la posición en operaciones de doblado de materiales. 

## Tipos de Movimientos en el Control de Movimiento

- **Movimiento Lineal**: Desplazamiento en línea recta.
- **Movimiento Rotacional**: Giro alrededor de un eje.
- **Movimiento Combinado**: Integración de movimientos lineales y rotacionales para lograr trayectorias complejas.

## Ejemplo: Impresoras

En las impresoras, el control de movimiento es esencial para:

- **Posicionamiento del Cabezal de Impresión**: Mover el cabezal a lo largo del papel con precisión.
- **Alimentación del Papel**: Controlar el avance del papel para asegurar una impresión uniforme.


## Evolución del Control de Movimiento

### Antes del Control de Movimiento Moderno

- **Uso de Motores Grandes**: Se empleaban motores de gran tamaño para accionar múltiples mecanismos.
- **Engranajes y Transmisiones Mecánicas**: Complejos sistemas de engranajes transmitían el movimiento desde un único motor a diferentes partes de la máquina.

### Mejoras con el Control de Movimiento

- **Precisión Incrementada**: Los sistemas modernos permiten un control más exacto de posiciones y velocidades.
- **Reducción de Tamaño y Complejidad**: Se utilizan motores más pequeños y sistemas electrónicos, disminuyendo la necesidad de engranajes voluminosos.
- **Flexibilidad Operativa**: Es más sencillo reprogramar y adaptar máquinas para diferentes tareas sin modificaciones mecánicas extensas.


  ![Figura 1](imagenes/impresora.png) 

Figura 1. Diagrama de una impresora mostrando los componentes controlados por sistemas de movimiento. ([Fuente](https://quecartucho.es/blog/partes-de-una-impresora/))

  ![Figura 2](imagenes/dobladora.png)![Figura 2](imagenes/dobla.png)
  
Figura 2. Imagen comparativa entre una máquina antigua con múltiples engranajes y una moderna con control de movimiento avanzado (CNC).([Fuente1](https://download.e-bookshelf.de/download/0003/9488/62/L-G-0003948862-0008296858.pdf))([Fuente2](https://aeromaquinados.com/product/dobladoras-de-lamina-cnc-80t-2500/))


Estas figuras ayudarán a visualizar los conceptos y la evolución en el control de movimiento dentro de diversas aplicaciones industriales.

## Conceptos Claves en el Control de Movimiento

## ¿Qué es un Actuador (Motor)?

Un **actuador** es un dispositivo que convierte energía en movimiento. En el contexto del control de movimiento, el actuador más común es el **motor**, que puede ser:

![Figura 3](imagenes/motor.png)

Figura 3. actuadores.([Fuente](https://funciondelaindustria.wordpress.com/2017/05/10/los-motores-electricos-y-su-importancia-en-la-industria/))

## ¿Qué es un HMI?

Un **HMI (Human-Machine Interface)** es una interfaz que permite a los operadores comunicarse con un sistema de control de movimiento. Puede incluir:

- **Pantallas táctiles** con información en tiempo real.
- **Botones físicos y diales** para control manual.
- **Software SCADA** para supervisión y análisis de datos.

El HMI facilita la configuración, monitoreo y ajuste de parámetros en sistemas automatizados.

![Figura 4](imagenes/HMI.png)

Figura 4. HMI (Human-Machine Interface).([Fuente](https://grupo-syz.com/todos-los-productos/automatizacion/inferfaz-hombre-maquina-hmi/))


## Problemas Comunes en el Control de Movimiento

El control de movimiento puede enfrentar diversos problemas, entre ellos:

### 1. **Errores de Posicionamiento**
   - Causados por imprecisiones en sensores o desajustes mecánicos.
   - Se pueden corregir con sistemas de retroalimentación como encoders.

### 2. **Vibraciones y Resonancias**
   - Ocurren cuando el sistema mecánico no está bien amortiguado.
   - Se solucionan con ajuste de parámetros PID o uso de materiales adecuados.

### 3. **Sobrecalentamiento de Motores**
   - Puede deberse a un dimensionamiento incorrecto del motor.
   - Se mitiga con ventilación, disipadores de calor o selección de motores más eficientes.

### 4. **Fallas en la Comunicación**
   - Conexiones inadecuadas o interferencias pueden causar pérdida de datos.
   - Se previenen con cableado de calidad y protocolos de comunicación robustos.

### 5. **Fallas en la Fuente de Alimentación**
   - Un suministro inestable puede afectar el rendimiento del sistema.
   - Uso de reguladores de voltaje y fuentes de alimentación adecuadas minimizan este problema.

## Otras Aplicaciones del Control de Movimiento

Además de las impresoras, cortadoras y máquinas dobladoras, el control de movimiento se encuentra en:

| Aplicación                 | Descripción                                                                 |
|----------------------------|-----------------------------------------------------------------------------|
| **Robótica Industrial**    | Control preciso de brazos robóticos en líneas de ensamblaje.               |
| **Vehículos Autónomos**    | Sistemas de navegación en drones y robots móviles.                         |
| **Máquinas CNC**          | Fresado y torneado controlado por computadora.                              |
| **Impresión 3D**          | Movimiento preciso de extrusores para crear objetos en capas.               |
| **Ascensores**            | Regulación de la velocidad y posicionamiento de cabinas.                    |
| **Sistemas de Embalaje**  | Movimiento sincronizado de productos en líneas de producción.               |

Tabla 1. Aplicaciones del Control de Movimiento

El control de movimiento es fundamental en la automatización moderna, optimizando precisión, velocidad y eficiencia en múltiples industrias.

## Ejercicios sobre Control de Movimiento

### Ejercicio 1: Cálculo de Velocidad en un Sistema de Control de Movimiento

Un motor mueve una cinta transportadora con una velocidad angular de $$\omega = 10 $$ rad/s. Si el radio del tambor que impulsa la cinta es de r = 0.15 m, determina la velocidad lineal de la cinta.

**Fórmula utilizada:**

$$
v = \omega \cdot r
$$

**Sustituyendo los valores:**

$$
v = (10 \text{ rad/s}) \cdot (0.15 \text{ m})
$$

$$
v = 1.5 \text{ m/s}
$$

**Respuesta:** La velocidad lineal de la cinta es **1.5 m/s**.

---

### Ejercicio 2: Cálculo de Torque en un Motor

Un servomotor aplica una fuerza de F = 50N en el extremo de un brazo de palanca de r = 0.2 m. Calcula el torque generado por el motor.

**Fórmula utilizada:**

$$
\tau = F \cdot r
$$

**Sustituyendo los valores:**

$$
\tau = (50 \text{ N}) \cdot (0.2 \text{ m})
$$

$$
\tau = 10 \text{ Nm}
$$

**Respuesta:** El torque generado por el motor es **10 Nm**.

### Ejercicio 3: Aceleración Angular en un Motor

Un motor eléctrico parte del reposo y alcanza una velocidad angular de $$\omega_f = 50$$ rad/s en un tiempo de  t = 5 s. Determina la aceleración angular necesaria para lograr este cambio de velocidad.

**Fórmula utilizada:**

$$
\alpha = \frac{\omega_f - \omega_0}{t}
$$

**Sustituyendo los valores:**

$$
\alpha = \frac{50 - 0}{5}
$$

$$
\alpha = 10 \text{ rad/s}^2
$$

**Respuesta:** La aceleración angular del motor es **10 rad/s²**.

---

### Ejercicio 4: Fuerza Necesaria para Acelerar un Carro con Control de Movimiento

Un sistema de control de movimiento en una línea de ensamblaje impulsa un carro de m = 200 kg con una aceleración de a = 2.5 m/s². Determina la fuerza que debe aplicar el sistema.

**Fórmula utilizada:**

$$
F = m \cdot a
$$

**Sustituyendo los valores:**

$$
F = (200 \text{ kg}) \cdot (2.5 \text{ m/s}^2)
$$

$$
F = 500 \text{ N}
$$

**Respuesta:** La fuerza necesaria para acelerar el carro es **500 N**.

## Conclusión

A lo largo de estos apuntes, aprendimos sobre el **control de movimiento** y su importancia en la automatización. Descubrimos cómo los motores, actuadores y HMI permiten un control preciso en diversas aplicaciones industriales, como impresoras, cortadoras y máquinas CNC. Entendimos cómo ha evolucionado este campo, pasando de sistemas mecánicos con grandes motores y engranajes a soluciones más eficientes y flexibles.  

Además, resolvimos ejercicios que nos ayudaron a aplicar conceptos clave, como el cálculo de velocidad, torque, aceleración angular y fuerza. Gracias a esto, ahora tenemos una mejor comprensión de cómo funciona el control de movimiento en la industria y cómo se pueden optimizar los sistemas para mejorar su desempeño.


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

![Figura 5](imagenes/control1.png)

Figura 5. Diagrama control PID.([Fuente](https://www.picuino.com/es/control-pid.html))

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

![Figura 6](imagenes/control2.png)

Figura 6. Diagrama control Cascada.  ([Fuente](https://controlautomaticoeducacion.com/control-realimentado/control-en-cascada/))


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
