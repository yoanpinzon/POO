# 🌿 **Las Cicatrices del Valle Iridiano**  
### *Proyecto Final de Programación Orientada a Objetos*

## 🕰️ **Fecha de Entrega:** *Según la fecha acordada en clase*

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

Perfecto, aquí tenés la sección de **Entregables del Proyecto** actualizada, quitando la mención a *GitHub Flow* pero manteniendo la estructura clara y profesional:

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

### 📊 Rúbrica de Evaluación del Proyecto

> Esta rúbrica se utilizará para evaluar tanto por parte del profesor como a través de una autoevaluación y coevaluación del equipo. Todos los equipos deben incluir un archivo `calificacion.md` en su repositorio con los puntajes propuestos por cada integrante.

---

| # | Criterio | Descripción | Puntaje Máx. | Niveles de Desempeño |
|---|----------|-------------|---------------|------------------------|
| 1 | **Herencia y Jerarquía de Clases** | Herencia de al menos dos niveles con una jerarquía clara y funcional. | 15 pts | **15 pts**: Hay al menos dos niveles de herencia correctamente implementados. Las relaciones entre clases son coherentes y se evidencia un diseño bien pensado.<br>**10 pts**: Se implementa herencia, pero falta profundidad o hay inconsistencias leves en la jerarquía.<br>**5 pts**: Se usó herencia de un solo nivel o con errores importantes.<br>**0 pts**: No hay herencia o su uso es incorrecto. |
| 2 | **Herencia Múltiple** | Al menos una clase hereda de dos clases base distintas. | 10 pts | **10 pts**: La herencia múltiple está correctamente aplicada y resuelta sin ambigüedades.<br>**6 pts**: Está presente pero presenta problemas menores o ambigüedad funcional.<br>**3 pts**: Implementación poco clara o forzada.<br>**0 pts**: No hay herencia múltiple. |
| 3 | **Polimorfismo** | Uso de métodos virtuales puros y sobreescritura para definir comportamientos en subclases. | 10 pts | **10 pts**: Métodos virtuales puros correctamente definidos y sobreescritos; se evidencia uso de polimorfismo dinámico.<br>**6 pts**: Uso parcial o limitado de virtuales (no puros), con polimorfismo incompleto.<br>**3 pts**: Uso incorrecto o poco funcional.<br>**0 pts**: No hay uso de métodos virtuales ni de polimorfismo. |
| 4 | **Composición y Agregación** | El mapa contiene nodos, y los nodos contienen criaturas. Las criaturas tienen objetos internos. | 10 pts | **10 pts**: El diseño demuestra una clara relación de composición y agregación con estructuras anidadas.<br>**6 pts**: Parcialmente implementado o con estructura algo rígida.<br>**3 pts**: Uso limitado o con errores de diseño.<br>**0 pts**: No hay composición o agregación significativa. |
| 5 | **Asociaciones entre Objetos** | Las criaturas interactúan sin poseerse directamente (punteros o referencias). | 5 pts | **5 pts**: Interacciones claras entre objetos independientes (ataques, alianzas, etc.).<br>**3 pts**: Asociaciones limitadas o ambiguas.<br>**1 pt**: Interacción casi inexistente.<br>**0 pts**: No hay asociación o es incorrecta. |
| 6 | **Uso de Contenedores STL** | Se aplican contenedores como `vector`, `map`, `queue`, etc. | 10 pts | **10 pts**: Uso acertado y eficiente de múltiples contenedores STL.<br>**6 pts**: Uso básico de `vector` y uno más.<br>**3 pts**: Solo `vector`, uso limitado o innecesario.<br>**0 pts**: No se utilizan contenedores STL. |
| 7 | **Números Aleatorios** | Uso de la librería `<random>` y sus componentes. | 5 pts | **5 pts**: Uso correcto de <random>.<br>**3 pts**: Uso limitado o con errores menores.<br>**1 pt**: Uso incorrecto o trivial.<br>**0 pts**: No se usa aleatoriedad. |
| 8 | **Diseño General y Organización** | Claridad, cohesión, separación de responsabilidades. | 10 pts | **10 pts**: Código modular, limpio y bien organizado.<br>**6 pts**: Buen diseño con algunos puntos de mejora.<br>**3 pts**: Diseño poco claro o monolítico.<br>**0 pts**: Diseño desorganizado o sin estructura. |
| 9 | **Funcionalidad General del Ecosistema** | Reglas de simulación, reproducción, muerte, mutación. | 15 pts | **15 pts**: Todas las funcionalidades del mundo están implementadas con éxito.<br>**10 pts**: Más del 75% implementado.<br>**5 pts**: Algunas funciones básicas están presentes.<br>**0 pts**: No hay funcionalidad clara. |
| 10 | **Documentación del Código** | Comentarios útiles, README, uso opcional de Doxygen. | 5 pts | **5 pts**: Código comentado, README completo y útil.<br>**3 pts**: Comentarios o README faltantes o superficiales.<br>**1 pt**: Pobre documentación.<br>**0 pts**: Sin documentación. |
| 11 | **Uso de GitHub y Gestión de Proyecto** | Pull requests, issues, ramas. | 5 pts | **5 pts**: Se cumple con todo: 5+ PRs, 20+ issues, ramas bien gestionadas.<br>**3 pts**: Uso parcial de herramientas.<br>**1 pt**: Repositorio desorganizado.<br>**0 pts**: Sin uso claro de GitHub. |

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

> [!IMPORTANT] 
>
> - **Uso de Inteligencia Artificial:** Está **completamente permitido** el uso de herramientas de inteligencia artificial para asistir en el desarrollo del proyecto. **No será penalizado** de ninguna manera. Lo único indispensable es que el grupo **comprenda el código generado** y sea capaz de **explicarlo en detalle** si se le solicita.
>
> - **Adecuación del Proyecto a las Capacidades del Grupo:** Cada grupo tiene **plena libertad para ajustar el alcance del proyecto** de acuerdo con sus conocimientos y habilidades actuales. 
