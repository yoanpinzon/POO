# 🌿 **Las Cicatrices del Valle Iridiano**  
### *Proyecto Final de Programación Orientada a Objetos*

![Version](https://img.shields.io/badge/version-1.2-blue)
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

Para garantizar una experiencia de desarrollo colaborativa, profesional y organizada, el equipo deberá cumplir con los siguientes entregables y lineamientos técnicos:

### 🧑‍🤝‍🧑 **Roles dentro del Equipo**

- **👨‍💻 Líder Técnico**:  
  - Responsable de revisar la calidad del código.  
  - Revisión y aprobación de *pull requests*.  
  - Integración de cambios en la rama principal (*merge*).  
  - Seguimiento de funcionalidades pendientes y mejoras.

- **📄 Responsable de Calidad y Documentación**:  
  - Garantiza la documentación del código.  
  - Uso sugerido (pero no obligatorio) de herramientas como **Doxygen**.  
  - Supervisa que cada módulo esté documentado correctamente.

- **👥 Desarrolladores**:  
  - Todos los miembros deben participar activamente en el desarrollo.  
  - Cada integrante será responsable de implementar distintas clases o funcionalidades clave del sistema.

---

### 🌐 **Organización del Proyecto en GitHub**

- Cada nueva funcionalidad o corrección debe desarrollarse en una rama separada.  
- No se deben eliminar las ramas luego del merge, para mantener trazabilidad del trabajo.  
- El repositorio debe incluir al menos:
  - ✅ **3 Pull Requests** con revisiones entre compañeros.  
  - ✅ **10 Issues** que reflejen las tareas, bugs o mejoras asignadas y resueltas.  
  - ✅ **README.md completo** actuando como **manual del proyecto**, con:
    - Descripción del proyecto y objetivos.  
    - Instrucciones de compilación y ejecución.  
    - Estructura de carpetas y explicación del código.  
    - Guía de contribución y uso de ramas.  
    - Créditos y roles del equipo.

---

### 📂 **Archivos obligatorios del repositorio**

El repositorio del proyecto debe incluir:

1️⃣ `README.md` obligatorio con:

  - 📘 **Descripción del proyecto**:  
    Breve explicación del propósito del sistema, el problema que resuelve y a quién está dirigido (usuarios objetivo).

  - 🧑‍💻 **Manual del usuario**:  
    Guía clara y amigable para entender cómo se utiliza la aplicación. Puede incluir:  
    - Principales funcionalidades y casos de uso.  
    - Instrucciones paso a paso para interactuar con la interfaz o los comandos.  
    - Capturas de pantalla o ejemplos de uso (si es posible).  
    - Requisitos mínimos para su uso (por ejemplo: navegador recomendado, permisos necesarios, resolución mínima, etc.).

  - 🛠️ **Instrucciones de compilación y ejecución** (si aplica):  
    - Cómo clonar el repositorio y preparar el entorno.  
    - Instalación de dependencias necesarias.  
    - Cómo compilar o ejecutar la aplicación localmente (según el lenguaje y entorno usados).

  - 🗂️ **Estructura del código fuente**:  
    - Descripción de la organización general del código.  
    - Carpetas principales.  
    - Breve mención de los módulos o clases clave del sistema.

  - 👥 **Créditos y roles del equipo**:  
    - Lista de integrantes del grupo.  
    - Tareas o responsabilidades principales que asumió cada persona durante el proyecto.

2️⃣ `calificacion.md`: Autoevaluaciones y coevaluaciones de cada miembro del grupo.

3️⃣ `uml.md`:  
  Documento en **formato Markdown** con el **diagrama de clases UML** realizado utilizando **Mermaid**. Este archivo debe reflejar las relaciones entre clases, herencias, asociaciones, composición y cualquier otro aspecto clave del diseño orientado a objetos del sistema.

> [!NOTE]
> ✅ El `README.md` debe estar bien redactado, claro, y ser útil tanto para **usuarios finales** como para **desarrolladores** que quieran revisar o continuar el proyecto.

### 📊 Rúbrica de Evaluación del Proyecto

> Esta rúbrica se utilizará para evaluar tanto por parte del profesor como a través de una autoevaluación y coevaluación del equipo. Todos los equipos deben incluir un archivo `calificacion.md` en su repositorio con los puntajes propuestos por cada integrante.

---

| # | Criterio | Descripción | Puntaje Máx. | Niveles de Desempeño |
|---|----------|-------------|---------------|------------------------|
| 1️⃣ | **Uso de GitHub y Gestión del Proyecto** | Uso activo de ramas, issues, revisiones y documentación del repositorio. | 10 pts | **10 pts**: Al menos 3 pull requests revisados, 10 issues con tareas y bugs resueltos, ramas separadas por funcionalidad.<br>**6 pts**: Uso parcial de PRs o issues, documentación mínima.<br>**3 pts**: Repositorio caótico o con poco uso de herramientas colaborativas.<br>**0 pts**: Sin trazabilidad ni gestión colaborativa. |
| 2️⃣ | **Herencia y Jerarquía de Clases** | Uso adecuado de herencia con jerarquía funcional y coherente. | 10 pts | **10 pts**: Dos niveles o más de herencia correctamente implementados y con propósito claro.<br>**6 pts**: Herencia básica o con errores leves en la jerarquía.<br>**3 pts**: Herencia superficial o forzada.<br>**0 pts**: No hay herencia o es incorrecta. |
| 3️⃣ | **Composición, Agregación y Asociación** | Relaciones entre objetos claramente diferenciadas y correctamente modeladas. | 10 pts | **10 pts**: El diseño evidencia relaciones de composición, agregación y asociaciones funcionales entre objetos.<br>**6 pts**: Relaciones están presentes, pero con ambigüedad o diseño rígido.<br>**3 pts**: Relaciones poco claras o inconsistentes.<br>**0 pts**: No se evidencia ningún tipo de relación entre objetos. |
| 4️⃣ | **Polimorfismo** | Uso de métodos virtuales y sobreescritura en subclases. | 10 pts | **10 pts**: Métodos virtuales correctamente usados con sobreescritura coherente y polimorfismo dinámico funcional.<br>**6 pts**: Polimorfismo presente pero con errores menores o limitado.<br>**3 pts**: Implementación incorrecta o poco efectiva.<br>**0 pts**: No se aplica polimorfismo. |
| 5️⃣ | **Uso de Contenedores STL** | Aplicación correcta y efectiva de estructuras de datos estándar. | 10 pts | **10 pts**: Uso pertinente de varios contenedores (`vector`, `map`, `queue`, etc.).<br>**6 pts**: Uso básico pero correcto.<br>**3 pts**: Uso innecesario o mal aplicado.<br>**0 pts**: No se usan contenedores STL. |
| 6️⃣ | **Uso de Aleatoriedad** | Generación de eventos o comportamientos aleatorios con <random>. | 5 pts | **5 pts**: Uso correcto y con propósito claro.<br>**3 pts**: Uso básico o con errores menores.<br>**1 pt**: Uso incorrecto o irrelevante.<br>**0 pts**: No se usa aleatoriedad. |
| 7️⃣ | **Persistencia de Datos** | Almacenamiento y recuperación de datos usando archivos o serialización. | 10 pts | **10 pts**: Guardado y carga implementados correctamente (archivos de texto, binarios, JSON, etc.).<br>**6 pts**: Persistencia funcional pero limitada.<br>**3 pts**: Presente pero poco útil o con errores.<br>**0 pts**: Sin persistencia. |
| 8️⃣ | **Diseño y Organización del Código** | Claridad del diseño, modularidad y organización de archivos. | 10 pts | **10 pts**: Código limpio, modular, con clases separadas en `.h` y `.cpp`. Arquitectura clara.<br>**6 pts**: Organización mayormente correcta, pero con algunas clases sin modularizar o archivos mal distribuidos.<br>**3 pts**: Diseño poco claro, muchas clases en el mismo archivo.<br>**0 pts**: Código desordenado, sin separación entre declaración e implementación. |
| 9️⃣ | **Manual del Usuario** | Guía clara y útil para el usuario final. | 15 pts | **15 pts**: Manual detallado con funcionalidades, casos de uso, capturas, requisitos, etc.<br>**10 pts**: Manual funcional pero con detalles faltantes.<br>**5 pts**: Muy básico o incompleto.<br>**0 pts**: No hay manual. |
| 🔟 | **Documentación del Código** | Comentarios útiles y buena legibilidad. | 5 pts | **5 pts**: Código comentado y entendible, sin excesos.<br>**3 pts**: Comentarios parciales o superficiales.<br>**1 pt**: Comentarios escasos o irrelevantes.<br>**0 pts**: Sin documentación. |
| 1️⃣1️⃣ | **README Técnico del Proyecto** | Archivo `README.md` completo con información técnica. | 5 pts | **5 pts**: Incluye descripción, instrucciones, estructura del código, guía de contribución, créditos, etc.<br>**3 pts**: Incompleto o desorganizado.<br>**1 pt**: Información mínima.<br>**0 pts**: No hay README o es irrelevante. |

✅ **Total: 100 puntos**

---

### 📝 Autoevaluación y Coevaluación (Incluidas en `calificacion.md`)

Cada miembro debe realizar dos evaluaciones:  
- Una **autoevaluación** de su propio desempeño ✅  
- Una **coevaluación** para cada uno de los demás miembros del equipo 👥”  

**Aspectos a evaluar (5 puntos cada uno):**
- Colaboración y trabajo en equipo
- Responsabilidad y compromiso
- Contribución técnica
- Uso consciente de asistentes de IA

Ejemplo de tabla para `calificacion.md`:

### ✅ Autoevaluación — *Juan Pérez*

| Criterio                          | Puntaje (1-5) | Comentarios breves                                 |
|----------------------------------|---------------|-----------------------------------------------------|
| Colaboración y trabajo en equipo | 5             | Fui puente de comunicación entre todos              |
| Responsabilidad y compromiso     | 4             | Cumplí, pero me costó con los commits a tiempo      |
| Contribución técnica             | 5             | Hice la parte de herencia múltiple y polimorfismo   |
| Uso de asistentes de IA          | 4             | Lo usé para revisar bugs y lo expliqué al equipo    |
| **Subtotal autoevaluación**      | **18 / 20**   |                                                     |

---

### 👤 Coevaluación — *María Gómez* (evaluada por Juan Pérez)

| Criterio                          | Puntaje (1-5) | Comentarios breves                          |
|----------------------------------|---------------|----------------------------------------------|
| Colaboración y trabajo en equipo | 5             | Siempre activa en las reuniones              |
| Responsabilidad y compromiso     | 5             | Entregó todo a tiempo                        |
| Contribución técnica             | 4             | Ayudó en STL y composición del mapa          |
| Uso de asistentes de IA          | 3             | Lo usó bien pero no siempre explicó su uso   |
| **Subtotal evaluación de Juan**  | **17 / 20**   |                                              |

---

### 🧾 Tabla resumen de coevaluación de María Gómez

| Evaluador     | Puntaje total sobre 20 |
|---------------|-------------------------|
| Juan Pérez    | 17                      |
| Diego Ruiz    | 18                      |
| **Promedio coevaluación** | **17.5 / 20**         |

---

### 🎯 Totales individuales (Juan Pérez)

| Evaluación       | Puntaje |
|------------------|---------|
| Autoevaluación   | 18      |
| Promedio Coevaluación (María + Diego) | 17.5    |
| **Promedio Final**     | **17.75 / 20** |

---

# 📅 Cronograma Completo de Sustentaciones

| Día | Hora | Grupo | Nombre del Grupo | Líder | Miembros |
|-----|------|--------|------------------|--------|-----------|
| mié. 30/04/2025 | 7:00 a. m. | 13 | Virtual insanity | Hanna Lozano Orozco | Valerie Marmolejo Molina |
| mié. 30/04/2025 | 7:30 a. m. | 11 | Sparkies VII | Juan Fernando Muñoz Lopez | Santiago Henao Ramirez |
| mié. 30/04/2025 | 8:00 a. m. | 2 | Cafe y depuración | Isabella Arango Moreno | Santiago Carvajal Chamorro |
| mié. 30/04/2025 | 8:30 a. m. | 5 | Los desprogramadores | Juan Jose Lopez Valencia | Martin Estrada Agudelo |
| vie. 02/05/2025 | 7:30 a. m. | 7 | Los pájaros | Juan Camilo Espinosa Arias | Juan Felipe Sanchez Morillo, Samuel Cuervo Peña |
| vie. 02/05/2025 | 8:00 a. m. | 9 | Objetos en evolución | Samuel Chacon Roman | Sebastian Duran Barros |
| vie. 02/05/2025 | 8:30 a. m. | 1 | .pinzon | Antonia Salguero Cortes | Juan Sebastian Silva Caicedo, Miguel Angel Rodriguez Bermudez |
| mié. 07/05/2025 | 7:30 a. m. | 6 | Los gepetos | Carlos David Sanchez Calderon | Emerson David Perea Mosquera, Juan Esteban Ramirez Delarosa, Pablo Tomas Bejarano Muñoz, Samuel David Mueses Cadavid, Samuel Eduardo Guzman Conde |
| mié. 07/05/2025 | 8:00 a. m. | 12 | Triple J | Jose Daniel Mesa Velasquez | Jose David Gonzalez Muñoz, Julian Andres Hurtado Florez |
| mié. 07/05/2025 | 8:30 a. m. | 4 | Las estrellitas flamantes | Isabella Garzon Salazar | Juan David Rojas Umaña |
| mié. 07/05/2025 | 9:00 a. m. | 8 | Los traquetos | Isabella Ramirez Echeverry | Juan Manuel Ramirez Gonzalez |
| vie. 09/05/2025 | 7:30 a. m. | 10 | Sapiens | David Avila Rodriguez | Sara Isabel Orrego Gallego |
| vie. 09/05/2025 | 8:00 a. m. | 3 | Crínima 2.1 | Cristian Miguel Hoyos Leon | Maria Isabel Solis Gonzalez, Nicolle Stheyzy Ureña Garcia |
| vie. 09/05/2025 | 8:30 a. m. | 14 | YuPro | Shi Jian Alejandro Yu Chen | *(Sin miembros adicionales registrados)* |

---

> [!IMPORTANT] 
>
> - **Uso de Inteligencia Artificial:** Está **completamente permitido** el uso de herramientas de inteligencia artificial para asistir en el desarrollo del proyecto. **No será penalizado** de ninguna manera. Lo único indispensable es que el grupo **comprenda el código generado** y sea capaz de **explicarlo en detalle** si se le solicita.
>
> - **Adecuación del Proyecto a las Capacidades del Grupo:** Cada grupo tiene **plena libertad para ajustar el alcance del proyecto** de acuerdo con sus conocimientos y habilidades actuales. 
