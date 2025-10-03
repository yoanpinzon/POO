# 🏆 **Proyecto Final — Programación Orientada a Objetos — 2025-02**

### 🌿 *Las Cicatrices del Valle Iridiano*

![Version](https://img.shields.io/badge/version-1.4-blue)
[![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg?color=#007ec6)](https://creativecommons.org/licenses/by-nc-nd/4.0/)


## 🕰️ **Fecha de Entrega:** [Ver cronograma al final](#-cronograma-completo-de-sustentaciones)

---

## 📖 **Sinopsis General**

*“Las Cicatrices del Valle Iridiano”* es más que un título: es el corazón del universo que vas a programar. Este proyecto final propone la construcción de un ecosistema narrativo, vivo, impredecible y lleno de interacciones, donde el diseño orientado a objetos no es solo una herramienta, sino el lenguaje que da vida a un mundo en constante transformación. 

Como programador/a, serás el arquitecto de Sangara, un sistema biológico complejo que refleja las tensiones entre equilibrio, evolución y colapso. Cada clase, cada objeto, cada decisión en tu diseño tendrá un impacto directo en el desarrollo de este universo ficticio. 

---

## 🌌 **El Valle Iridiano: Una Historia Viva**

El Valle Iridiano no siempre fue una tierra fragmentada. Antaño, sus regiones —los Altos Cálidos, las Lomas Mansas, los Llanos Opacos y las Zonas Profundas— se encontraban en constante equilibrio, reguladas por una red viva de criaturas que habitaban bajo, sobre y dentro de la tierra. Estas criaturas, nacidas de la Convergencia, respondían al pulso vital del valle: un ciclo rítmico que definía sus comportamientos, necesidades y relaciones. Cada ciclo era como un latido: con él, las criaturas comían, se movían, se reproducían o morían.

Ese equilibrio se rompió con la aparición de los **Anómalos**, seres que no respondían al pulso. Nadie sabe cómo llegaron, pero su presencia alteró el ecosistema. Algunos nodos del valle —pequeñas regiones conectadas por senderos naturales— comenzaron a enfermar; otros simplemente se vaciaron. El pulso ya no llegaba a todos por igual. 

El Observador, un ente que nunca había intervenido, fue despertado. Su rol era vigilar, documentar y, en última instancia, restaurar. Para ello, debía comprender nuevamente el entramado vital del valle.

En su primer día de observación, notó que en los nodos aún activos convivían varias criaturas. Cada una respondía al pulso a su manera. Algunas se arrastraban lentamente sobre las rocas —eran los **Lentos de Raíz**, criaturas que solo lograban reproducirse si habían permanecido estables durante muchos ciclos. Otras brillaban brevemente al moverse: eran las **Centellas**, rápidas y de vida breve, capaces de generar copias de sí mismas si encontraban nodos iluminados.

Los **Metamorfitas**, por su parte, se adaptaban al entorno. Si el nodo en el que habitaban era seco, mutaban; si era cálido, adquirían nuevas defensas. El Observador notó con atención creciente a una criatura en particular: el **Albo**, que no solo se adaptaba, sino que también se desplazaba y replicaba nodos vecinos cuando encontraba condiciones óptimas. El Albo parecía poseer habilidades tanto de las Centellas como de los Metamorfitas, algo nunca antes visto. Su existencia misma demostraba una fusión: una nueva etapa evolutiva.

El Observador decidió registrar todos los comportamientos. En cada pulso, visitaba todas las criaturas: observaba si seguían vivas, si se desplazaban a nodos vecinos, si se multiplicaban o si perecían. Algunas dejaban residuos que modificaban el ambiente. Un nodo que albergaba una criatura durante muchos ciclos cambiaba su estado: se volvía fértil, letal o incluso corrupto.

Y así, cada criatura no solo afectaba el entorno: el entorno también las moldeaba.

El Observador clasificó a las criaturas. No por capricho, sino por necesidad. Las agrupó por su comportamiento base: las **Raíz** eran estáticas, pero fértiles. Las **Chispa**, móviles y breves. Las **Cambio**, moldeables y variables. Cada categoría incluía múltiples especies, cada una con propiedades particulares. Algunas especies tenían órganos internos —núcleos, cámaras, membranas— que influían en cómo respondían al ciclo vital. Otras cargaban parásitos, o se acompañaban de entidades menores. El Observador debía registrarlo todo. 

En su segundo ciclo de observación, el Observador advirtió que el número de criaturas disminuía, y que algunas comenzaban a actuar con hostilidad. Un nodo, invadido por Alboides, parecía haber cortado el pulso vital. Las criaturas en su interior actuaban de forma errática, y aquellas que nacían allí lo hacían ya deformes. El Observador comprendió que no solo debía observar: debía decidir qué criaturas preservar y cuáles aislar. Para ello, debía almacenar su conocimiento, recuperar sesiones previas y simular escenarios.

Los días pasaban. El valle cambiaba. Las criaturas evolucionaban. Y el Observador, aunque nunca visible, dejaba su rastro en la arquitectura del mundo: modificando, limpiando, expandiendo. Era él quien decidía cuándo iniciar un nuevo ciclo, con qué criaturas, y qué nodos activar.

Pero a medida que más ciclos pasaban, el Observador comprendía una verdad más profunda: las criaturas no eran simples entes independientes. Algunas llevaban dentro de sí otras más pequeñas, que condicionaban su comportamiento. Otras, al morir, dejaban fragmentos que podían ser usados por futuras generaciones. Unas cuantas, incluso, establecían vínculos temporales entre sí, afectando mutuamente su supervivencia. Y algunas, como el Albo, eran producto de una herencia dual: nacidas del cruce improbable entre dos líneas antes incompatibles. 

El Observador supo entonces que su misión no era solo restaurar el valle. Era comprenderlo, codificarlo y enseñarlo. Porque para sanar Sangara, primero debía aprender a modelarlo.

---

## 💻 **Tu Misión como Desarrollador**

Debes construir una simulación basada en los principios de la programación orientada a objetos que refleje el comportamiento de las criaturas del valle, su entorno y los cambios que emergen con el tiempo. Esta simulación debe incluir:

- Un **mapa dinámico** representado como una matriz o red de nodos.
- Un conjunto inicial de criaturas, cada una con atributos particulares.
- Un sistema de **ciclos de vida**, donde las criaturas se reproducen, evolucionan, mueren o mutan.
- Cambios en el entorno que influyen en el comportamiento de los seres vivientes.
- Persistencia de los datos del mundo y sus criaturas mediante **JSON o XML**.

---

## 🧬 **Aspectos Técnicos Obligatorios**

Tu sistema debe aplicar claramente los siguientes conceptos de POO:

- **🧬 Herencia**: Las criaturas del mundo deben derivar de una clase base común, como `Criatura`, que contenga los atributos y comportamientos esenciales. A partir de allí, deben surgir al menos **dos niveles jerárquicos** de herencia (por ejemplo, `Criatura` → `Mutante` → `MutanteAlado`).

- **🔀 Herencia múltiple**: Al menos una clase deberá heredar de **dos clases base distintas**, como por ejemplo una criatura que hereda tanto de `Volador` como de `Regenerador`, con lógica clara para evitar ambigüedades.

- **🎭 Polimorfismo**: Se deben utilizar métodos virtuales puros en la clase base para definir comportamientos genéricos como `actuar()`, `reproducirse()`, `moverse()`, `morir()`, que serán sobreescritos por cada subclase para representar su lógica específica.

- **🧱 Agregación y/o Composición**: El **mapa del mundo** debe estar compuesto por una estructura de `Nodos` o `Celdas`, y cada nodo debe contener una o más criaturas. Las criaturas también pueden contener objetos internos que representen su estado energético, historial o evolución. Esto implica una composición clara entre clases.

- **🔗 Asociación simple**: Las criaturas deben poder interactuar con otras (por ejemplo, atacar, infectar, aliarse), sin poseerlas directamente. Esta relación debe representarse mediante punteros o referencias, dejando clara la independencia entre los objetos asociados.

- **📦 Uso de STL**: Se deben emplear contenedores como `vector`, `map`, `set` o `queue` para gestionar listas de criaturas, eventos o relaciones del ecosistema, asegurando un manejo dinámico y eficiente de la información.

- **🎲 Generador de números aleatorios**: Se debe usar la biblioteca `<random>` para definir comportamientos impredecibles como movimientos, mutaciones o eventos del entorno, asegurando realismo y variedad en la simulación.
  
- **🗂️ Persistencia**: El estado del ecosistema debe poder guardarse y recuperarse utilizando **serialización en JSON o XML**, permitiendo reanudar la simulación desde un punto anterior. Esto incluye guardar criaturas, posiciones, estados y vínculos relevantes.

---

## 🌿 **Un Mundo en Constante Transformación**

Cada iteración de tu programa (ciclo o “turno”) debe visitar todas las criaturas del mapa. En función de su estado, posición y entorno, decidirán si viven, mueren, migran, mutan o se reproducen. Esto convierte tu mundo en un sistema vivo inspirado, si querés, en *El Juego de la Vida* de Conway, pero con reglas y clases mucho más ricas.

La forma en que representás visualmente tu mapa o el estado de las criaturas queda a tu elección, pero debe ser clara, informativa y coherente con el modelo diseñado.

---

## 📦 **Entregables del Proyecto**

Para garantizar una experiencia de desarrollo profesional, organizada y completa, **cada estudiante** deberá cumplir con los siguientes entregables y lineamientos técnicos:

---

### 🌐 **Organización del Proyecto en GitHub**

* Cada estudiante debe trabajar en su **propio repositorio individual**.
* El repositorio debe incluir al menos:

  * ✅ **README.md completo**, actuando como **manual del proyecto**, con:

    * Descripción y objetivos del sistema.
    * Instrucciones de compilación y ejecución.
    * Estructura de carpetas y explicación del código.
    * Capturas de pantalla o ejemplos de uso (si aplica).
    * Créditos (autor del proyecto).
  * ✅ **Issues** que reflejen tareas o mejoras realizadas.
  * ✅ Uso de ramas opcional, pero recomendable para organizar cambios.

---

### 📂 **Archivos obligatorios del repositorio**

1️⃣ `README.md`:

* 📘 **Descripción del proyecto**: propósito del sistema, problema que resuelve y usuarios objetivo.
* 🧑‍💻 **Manual del usuario**: guía clara con funcionalidades principales, casos de uso e instrucciones paso a paso.
* 🛠️ **Instrucciones de compilación y ejecución** (cómo clonar, dependencias, cómo correr el proyecto).
* 🗂️ **Estructura del código fuente**: descripción de carpetas, clases principales y sus responsabilidades.
* 👤 **Autoría**: nombre completo del estudiante.

2️⃣ `calificacion.md`:

* Documento donde el estudiante realiza su **autoevaluación personal** (ver rúbrica).

3️⃣ `uml.md`:

* Diagrama de clases en **formato Markdown**, usando **Mermaid**.
* Debe reflejar herencias, asociaciones, composición y demás relaciones del diseño orientado a objetos.

> [!NOTE]
> ✅ El `README.md` debe ser claro y útil tanto para **usuarios finales** como para **otros desarrolladores**.

---

### 📊 Rúbrica de Evaluación del Proyecto

| #      | Criterio                                 | Descripción                                                          | Puntaje Máx. | Niveles de Desempeño                                                                                                                            |
| ------ | ---------------------------------------- | -------------------------------------------------------------------- | ------------ | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| 1️⃣    | **Uso de GitHub y Gestión del Proyecto** | Buen manejo del repositorio (issues, commits claros, documentación). | 10 pts       | **10**: Uso activo y ordenado.<br>**6**: Uso parcial o poco claro.<br>**3**: Uso mínimo.<br>**0**: No hay evidencia.                            |
| 2️⃣    | **Herencia y Jerarquía de Clases**       | Jerarquía funcional y coherente.                                     | 10 pts       | **10**: Dos o más niveles correctos.<br>**6**: Herencia básica o con errores leves.<br>**3**: Forzada o superficial.<br>**0**: No hay herencia. |
| 3️⃣    | **Composición, Agregación y Asociación** | Relaciones entre objetos correctamente modeladas.                    | 10 pts       | **10**: Correctas y diferenciadas.<br>**6**: Presentes pero ambiguas.<br>**3**: Poco claras.<br>**0**: No existen.                              |
| 4️⃣    | **Polimorfismo**                         | Uso correcto de métodos virtuales y sobreescritura.                  | 10 pts       | **10**: Implementación sólida.<br>**6**: Con errores menores.<br>**3**: Mal aplicado.<br>**0**: Ausente.                                        |
| 5️⃣    | **Uso de Contenedores STL**              | Aplicación de `vector`, `map`, `queue`, etc.                         | 10 pts       | **10**: Uso variado y pertinente.<br>**6**: Uso básico.<br>**3**: Mal aplicado.<br>**0**: No usados.                                            |
| 6️⃣    | **Uso de Aleatoriedad**                  | Generación de eventos o comportamientos aleatorios.                  | 5 pts        | **5**: Correcto y con propósito.<br>**3**: Básico o limitado.<br>**1**: Incorrecto.<br>**0**: No usado.                                         |
| 7️⃣    | **Persistencia de Datos**                | Guardado y carga de información.                                     | 10 pts       | **10**: Implementado correctamente.<br>**6**: Funcional pero limitado.<br>**3**: Poco útil.<br>**0**: Ausente.                                  |
| 8️⃣    | **Diseño y Organización del Código**     | Modularidad, claridad y limpieza.                                    | 10 pts       | **10**: Código limpio y modular.<br>**6**: Mayormente correcto.<br>**3**: Poco claro.<br>**0**: Desordenado.                                    |
| 9️⃣    | **Manual del Usuario**                   | Guía para el uso del sistema.                                        | 15 pts       | **15**: Completo y detallado.<br>**10**: Funcional pero incompleto.<br>**5**: Básico.<br>**0**: Ausente.                                        |
| 🔟     | **Documentación del Código**             | Comentarios útiles y legibles.                                       | 5 pts        | **5**: Bien comentado.<br>**3**: Parcial.<br>**1**: Escaso.<br>**0**: Ninguno.                                                                  |
| 1️⃣1️⃣ | **README Técnico del Proyecto**          | Información técnica completa.                                        | 5 pts        | **5**: Muy completo.<br>**3**: Incompleto.<br>**1**: Mínimo.<br>**0**: Ausente.                                                                 |

✅ **Total: 100 puntos**

---

### 📝 Autoevaluación Individual (en `calificacion.md`)

Cada estudiante debe realizar una **autoevaluación personal**, basada en los criterios de la rúbrica.

Ejemplo:

| Criterio                     | Puntaje (1-5) | Comentarios                                                    |
| ---------------------------- | ------------- | -------------------------------------------------------------- |
| Responsabilidad y compromiso | 5             | Cumplí con los plazos y entregué completo.                     |
| Diseño orientado a objetos   | 4             | Implementé herencia y polimorfismo, aunque podría refinar más. |
| Documentación                | 5             | Código y README claros.                                        |
| Uso consciente de IA         | 4             | Lo usé solo como apoyo, no para generar todo el código.        |
| **Subtotal autoevaluación**  | **18 / 20**   | —                                                              |

---

# 📅 Cronograma Completo de Sustentaciones

## ✅ **Martes 04-nov-2025**

| Hora          | Estudiante                  |
| ------------- | --------------------------- |
| 9:00 – 9:20   | Christian David Ruiz Medina |
| 9:20 – 9:40   | David Gaviria Leiton        |
| 9:40 – 10:00  | Derik Camilo Muñoz Calderon |
| 10:00 – 10:20 | Esteban Posso Orozco        |
| 10:20 – 10:40 | Juan David Narvaez Gelpud   |
| 10:40 – 11:00 | Juan Esteban Marin Cardona  |

---

## ✅ **Viernes 07-nov-2025**

| Hora          | Estudiante                    |
| ------------- | ----------------------------- |
| 11:00 – 11:20 | Juan Esteban Ramirez Delarosa |
| 11:20 – 11:40 | Juan Felipe Castillo Castaño  |
| 11:40 – 12:00 | Juan Jose Larrahondo Giron    |
| 12:00 – 12:20 | Juan Jose Rojas Canencio      |
| 12:20 – 12:40 | Juan Manuel Camacho Ibarguen  |
| 12:40 – 1:00  | Juan Miguel Caceres Catolico  |

---

## ✅ **Martes 11-nov-2025**

| Hora          | Estudiante                     |
| ------------- | ------------------------------ |
| 9:00 – 9:20   | Juan Pablo Toro Ruiz           |
| 9:20 – 9:40   | Julian Andres Rodriguez Castro |
| 9:40 – 10:00  | Leidy Jimena Caso Piamba       |
| 10:00 – 10:20 | Maria Camila Gaitan Angel      |
| 10:20 – 10:40 | Moises Agudelo Ocampo          |
| 10:40 – 11:00 | Nikolas Jimenez Sanchez        |

---

## ✅ **Viernes 14-nov-2025**

| Hora          | Estudiante                |
| ------------- | ------------------------- |
| 11:00 – 11:20 | Samuel Muñoz Quiroga      |
| 11:20 – 11:40 | Santiago Lasso Garcia     |
| 11:40 – 12:00 | Santiago Mazo Andrade     |
| 12:00 – 12:20 | Thomas David Gomez Tamayo |

---

### 🏆 **Criterios de Calificación y Sustentación**

La calificación del proyecto se compone de **dos partes complementarias**:

1. **Entregables en GitHub (0 a 5.0):**
   Incluye el repositorio, `README.md`, UML, documentación, manual del usuario, autoevaluación, etc. Esta parte refleja la calidad técnica y de organización del trabajo realizado.

2. **Sustentación individual (factor entre 0.0 y 1.0):**
   Durante la presentación, cada estudiante deberá **defender su proyecto** respondiendo a preguntas y explicando su propio código.

   * El factor puede tomar **cualquier valor decimal entre 0.0 y 1.0**, de acuerdo con la claridad, seguridad y profundidad de las respuestas.
   * Un dominio sobresaliente se acerca a **1.0**.
   * Un desempeño parcial puede ubicarse en valores como **0.7, 0.5, 0.3**, etc.
   * Una sustentación muy deficiente puede recibir incluso **0.0**.

3. **Nota final:**
   La nota definitiva se calcula multiplicando:

   [
   \text{Nota final} = \text{Nota entregables} \times \text{Factor sustentación}
   ]

   #### 🔢 Ejemplos ilustrativos

   * Nota en GitHub: **4.5** → Sustentación: **0.9** → Nota final: **4.1**
   * Nota en GitHub: **4.2** → Sustentación: **0.5** → Nota final: **2.1**
   * Nota en GitHub: **3.8** → Sustentación: **1.0** → Nota final: **3.8**
   * Nota en GitHub: **4.0** → Sustentación: **0.0** → Nota final: **0.0**

📌 **Importante:** La **nota final siempre se expresará con una sola cifra decimal (una décima)**.

---


> [!IMPORTANT] 
>
> - **Uso de Inteligencia Artificial:** Está **completamente permitido** el uso de herramientas de inteligencia artificial para asistir en el desarrollo del proyecto. **No será penalizado** de ninguna manera. Lo único indispensable es que el grupo **comprenda el código generado** y sea capaz de **explicarlo en detalle** si se le solicita.
>
> - **Adecuación del Proyecto a las Capacidades del Grupo:** Cada grupo tiene **plena libertad para ajustar el alcance del proyecto** de acuerdo con sus conocimientos y habilidades actuales. 
