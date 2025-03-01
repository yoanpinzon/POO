# **🧮 Tarea 3 - Acercandonos al Examen**

[![Unirse a la tarea](https://img.shields.io/badge/%F0%9F%91%89%20Unirse%20a%20la%20tarea%20en%20GitHub%20Classroom-blue?style=for-the-badge)](https://classroom.github.com/a/sHyJsgJf)

## **📢🚨 FECHA LÍMITE: Lunes 24 de febrero - 11:59 PM 🚨📢** <!-- omit in toc -->

⚠️ **ENTREGAS FUERA DE TIEMPO NO SERÁN ACEPTADAS.**  
✅ **Haz `commit` y `push` antes del plazo y verifica tu entrega en GitHub Classroom.**

---

## **📖 Descripción de la Tarea** <!-- omit in toc -->

## **📌 Problema (100 puntos) Guardianes de la Ciudad Flotante**  <!-- omit in toc -->

### **📖 Historia**

**Resumen:**  

En la ciudad flotante, los robos han aumentado y los **robots de respuesta** han sido activados para investigar. Construida hace siglos por una civilización avanzada que dominaba la gravedad, la metrópolis se mantiene suspendida gracias a una fuente cuántica de energía.  

La ciudad está organizada en **capas de sectores flotantes** en una cuadrícula **X × Y × Z**. Debido a restricciones gravitacionales, los robots **solo pueden cambiar de nivel en puntos de transición dispuestos en una espiral en sentido horario**.  

Un nuevo robo ha ocurrido en los niveles superiores, y un **robot de respuesta** ha sido enviado para actuar. Según su generación (**Modo Chester `M=0`**, **Modo Taka `M=1`**, **Modo Profesorcito `M=2`**), deberá moverse de la forma más eficiente para llegar al incidente.

Sin embargo, los registros de la red central indican que el robo fue denunciado **tres minutos antes de que ocurriera**, y una señal desconocida interfiere con las comunicaciones en ciertas partes de la ciudad. Nadie sabe quién envió la alerta… o si realmente hubo un robo.

---

### **📈 Movimientos del Robot**

Todos los índices en la ciudad comienzan desde `1`, no desde `0`. Es decir, la primera posición en cualquier dimensión `(X, Y, Z)` es `1`, y la última es `X_MAX`, `Y_MAX` o `Z_MAX`, respectivamente.

El robot puede moverse únicamente en las siguientes direcciones:
- **Izquierda** `(X-1, Y, Z)` (siempre que `X > 1`)
- **Derecha** `(X+1, Y, Z)` (siempre que `X < X_MAX`)
- **Arriba** `(X, Y+1, Z)` (siempre que `Y < Y_MAX`)
- **Abajo** `(X, Y-1, Z)` (siempre que `Y > 1`)

No está permitido moverse en diagonal ni salir de los límites de la ciudad.

---

### **📈 Modos de Respuesta ante Incidentes**

El robot puede desplazarse bajo tres modalidades:

1. (30 puntos) **Modo Taka (`M=0`)** → Se mueve en `X, Y` y usa los puntos de transición en espiral para cambiar de nivel `Z`.
2. (30 puntos) **Modo Chester (`M=1`)** → Se mueve en `X, Y` y usa los puntos de transición en espiral para cambiar de nivel `Z`, además de un portal que se encuentra en `(2,2,1)` y permite un salto instantáneo a `(2,2,Z_MAX)`. El robot debe decidir si utilizar el portal o los puentes en función de la distancia más corta.
3. (40 puntos) **Modo Profesorcito (`M=2`)** → Puede moverse libremente en `X, Y, Z`, sin necesidad de usar puntos de transición.

---

### **📁 Configuración de la Ciudad**&#x20;

1. **La ciudad tiene dimensiones `X × Y × Z`**.
2. **Los puntos de transición (puentes) están fijados en un patrón espiral en las esquinas**, siguiendo esta secuencia:
   - **Capa `Z=1`** → Puente en `(1,1)`, conecta con `Z=2`.
   - **Capa `Z=2`** → Puente en `(1,Y_MAX)`, conecta con `Z=3`.
   - **Capa `Z=3`** → Puente en `(X_MAX,Y_MAX)`, conecta con `Z=4`.
   - **Capa `Z=4`** → Puente en `(X_MAX,1)`, conecta con `Z=5`.
   - **El patrón se repite en espiral hasta `Z_MAX`**.
3. **Los puentes están predefinidos y no requieren configuración manual.** El costo de hacer uso del puente es 1. 
4. **El portal puede ser utilizado en el Modo Chester y se encuentra en `(2,2,1)`, permitiendo un salto instantáneo a `(2,2,Z_MAX)`, y viceversa.** El costo de uso del portal es `Z`. El robot debe evaluar si usar el portal o los puentes en función del menor costo.

---

### **📃 Entrada**

Todos los valores de `X`, `Y` y `Z` inician desde `1`, lo que significa que no hay coordenadas con índice `0` en la ciudad flotante.

El programa recibirá las siguientes entradas en este orden:

1. **CONFIGURAR X Y Z** → Define las dimensiones de la ciudad.
2. **UBICAR_ROBOT X Y Z M** → Coloca al robot en `(X, Y, Z)` con modo `M`.
3. **UBICAR_ROBO X Y Z** → Se conoce la ubicación exacta del incidente `(X, Y, Z)`.
4. **RUTA_MAS_CORTA** → Calcula la distancia mínima hasta el incidente.
5. **SALIR** → Finaliza el programa.

---

### **📌 Restricciones**  <!-- omit in toc -->

- **1 ≤ X ≤ 500** → Rango de X.  
- **1 ≤ Y ≤ 500** → Rango de Y.  
- **1 ≤ Z ≤ 500** → Rango de Z.  

---

### **📌 Salida**  <!-- omit in toc -->

El programa debe imprimir el resultado de los comandos indicados. 

---

### **Ejemplos de Entrada y Salida**  <!-- omit in toc -->

#### **Ejemplo Modo 0**<!-- omit in toc -->

##### Entrada:  <!-- omit in toc -->
```
CONFIGURAR 5 5 5
UBICAR_ROBOT 2 2 2 0
UBICAR_ROBO 3 3 4
RUTA_MAS_CORTA
SALIR
```  

##### Salida:  <!-- omit in toc -->
```
14
```  

---
#### **Ejemplo Modo 1**<!-- omit in toc -->

##### Entrada:  <!-- omit in toc -->
```
CONFIGURAR 5 5 5
UBICAR_ROBOT 3 1 1 1
UBICAR_ROBO 4 1 4
RUTA_MAS_CORTA
SALIR
```  

##### Salida:  <!-- omit in toc -->
```
13
```  

---
#### **Ejemplo Modo 2**<!-- omit in toc -->

##### Entrada:  <!-- omit in toc -->
```
CONFIGURAR 5 5 5
UBICAR_ROBOT 2 2 4 2
UBICAR_ROBO 3 3 1
RUTA_MAS_CORTA
SALIR
```  

##### Salida:  <!-- omit in toc -->
```
5
```  

---

## **📜 Notas Importantes**  <!-- omit in toc -->

- **El sistema debe manejar números grandes sin desbordarse.**  
- **El modo 1 debe evaluar si usar el portal o los puentes y elegir el menor costo.**  
- **El portal permite viajar entre los niveles `1` y `Z_MAX`, pero solo desde `(2,2)`.**  

---

### **📜 Código Base** <!-- omit in toc -->
El siguiente código base debe usarse para resolver este problema.  
⚠️ **No se debe cambiar el nombre del archivo, debe llamarse `main.cpp`.**  

```cpp
#include <iostream>

using namespace std;

// Definición de los límites máximos de la ciudad flotante
const int MAX_X = 500;
const int MAX_Y = 500;
const int MAX_Z = 500;

// Matriz tridimensional que representa la ciudad
int grid[MAX_X][MAX_Y][MAX_Z] = {};

// Vector que almacena las ubicaciones de los puentes en cada nivel Z (desde Z=1 hasta Z-1)
int puentes[MAX_Z][2];

// Variables globales para almacenar las dimensiones actuales de la ciudad
int X, Y, Z;

// Variables globales para almacenar la ubicación y modo del robot
int robotX, robotY, robotZ, robotM;

// Variables globales para la ubicación del incidente
int roboX, roboY, roboZ;

// Función para configurar la ciudad con las dimensiones dadas y establecer los puentes
void configurarCiudad(int x, int y, int z) {
    X = x; Y = y; Z = z;  // Asignar las dimensiones de la ciudad
    // TODO: Definir el patrón de espiral para los puntos de transición
    // TODO: Asignar los puntos de transición a los niveles correspondientes
}

// Función para calcular la ruta más corta en Modo 0
int calcularRutaMasCortaModo0() {
    // TODO: Implementar el algoritmo de búsqueda de ruta más corta para Modo 0
    return 0; // Retornar el resultado apropiado
}

// Función para calcular la ruta más corta en Modo 1
int calcularRutaMasCortaModo1() {
    // TODO: Implementar el algoritmo de búsqueda de ruta más corta para Modo 1
    return 0; // Retornar el resultado apropiado
}

// Función para calcular la ruta más corta en Modo 2
int calcularRutaMasCortaModo2() {
    // TODO: Implementar el algoritmo de búsqueda de ruta más corta para Modo 2
    return 0; // Retornar el resultado apropiado
}

// Función principal que inicia la ejecución del programa
int main() {
    string comando;
    while (cin >> comando) {
        if (comando == "CONFIGURAR") {  // Configurar la ciudad
            cin >> X >> Y >> Z;
            configurarCiudad(X, Y, Z);
        } else if (comando == "UBICAR_ROBOT") {  // Ubicar al robot
            cin >> robotX >> robotY >> robotZ >> robotM;
        } else if (comando == "UBICAR_ROBO") {  // Ubicar el incidente
            cin >> roboX >> roboY >> roboZ;
        } else if (comando == "RUTA_MAS_CORTA") {  // Calcular la ruta mínima según el modo
            if (robotM == 2) {
                cout << calcularRutaMasCortaModo2() << endl;
            } else if (robotM == 1) {
                cout << calcularRutaMasCortaModo1() << endl;
            } else {
                cout << calcularRutaMasCortaModo0() << endl;
            }
        } else if (comando == "SALIR") {  // Finalizar la ejecución
            break;
        }
    }
    return 0;
}
```

## **📌 ¿Cómo entregar la tarea en GitHub Classroom?** <!-- omit in toc -->

### **📝 Pasos para entregar tu código correctamente:** <!-- omit in toc -->

## 1️⃣ Aceptar la tarea  <!-- omit in toc -->
1. **Accede al enlace de la tarea:** [https://classroom.github.com/a/sHyJsgJf](https://classroom.github.com/a/sHyJsgJf).
2. **Acepta la tarea** haciendo clic en el botón correspondiente.  
3. Una vez aceptada, **se habrá creado automáticamente un repositorio en GitHub** con la siguiente dirección (reemplaza `TU_USUARIO` con tu nombre de usuario en GitHub):  
   ```
   https://github.com/profesorcito/tarea-3-TU_USUARIO
   ```
   Puedes verificarlo ingresando a tu cuenta de GitHub.  

## 2️⃣ Descargar el repositorio a tu computadora <!-- omit in toc -->  
4. **Abre Git Bash** en tu computadora.  
5. **Navega a la carpeta donde guardarás el proyecto** con el siguiente comando:  
   ```bash
   cd ~/Desktop/CLionProjects
   ```
6. **Clona tu repositorio** en tu computadora** con el siguiente comando (reemplaza `TU_USUARIO` con tu usuario en GitHub):  
   ```bash
   git clone https://github.com/profesorcito/tarea-3-TU_USUARIO.git
   ```

> [!NOTE]
>  
> Si tienes dudas sobre la dirección exacta del repositorio, **puedes copiarla desde GitHub** haciendo clic en el botón verde que dice **"Code"**.
>  
   

## 3️⃣ Abrir el repositorio en CLion <!-- omit in toc -->
7. **Abrir el proyecto en CLion**  
   - Presiona `Alt + F`.  
   - Selecciona **New** → **Project**.  
   - En la parte izquierda, selecciona **C++ Executable**.  
   - Busca la carpeta donde quedó el repositorio dentro de `CLionProjects`.  
   - Debe llamarse:  
     ```
     tarea-3-TU_USUARIO
     ```
   - Haz clic en **Create**.  

> [!IMPORTANT]
>
> Aparecerá un mensaje preguntando si deseas crear el proyecto sobre los archivos existentes. **Debes aceptar.**  Si pregunta si quieres abrirlo en esta ventana, **también acepta.**  
>

## 4️⃣ Modificar y probar el código <!-- omit in toc --> 
8. **Editar y ejecutar `main.cpp`:**  
   - Busca `main.cpp` y ábrelo.  
   - Escribe el código necesario para resolver el problema.  
   - Ejecuta el programa y verifica que la salida sea la esperada.  

## 5️⃣ Subir los cambios a GitHub <!-- omit in toc -->
10. **Guarda los cambios y súbelos a GitHub** con los siguientes comandos:  
   ```bash
   git add .
   git commit -m "Intento 1"
   git push origin master
   ```

> [!WARNING] 
> 
> Si el comando `git push` falla, es probable que el repositorio remoto haya sido modificado automáticamente, por ejemplo, por el bot de autograding. Para sincronizar tu repositorio local con estos cambios, ejecuta primero `git pull`. Esto traerá las actualizaciones más recientes y te permitirá integrar los cambios antes de intentar nuevamente el `git push`.
> 

## 6️⃣ Verificar la tarea en GitHub Classroom <!-- omit in toc -->  
11. **Revisa en la pestaña "Actions"** de GitHub si tu tarea fue aceptada.  
   - Si tu tarea fue aceptada, **se mostrará en verde** ✅.  
   - Si hubo errores, **se mostrará en rojo** ❌.  
12. Si haces clic en el último commit, puedes acceder a **"run-autograding-test"** para ver qué pruebas no pasaste.  
13. **Corrige el código y sube los cambios nuevamente** usando `git push` hasta que tu evaluación esté en verde.  

---
> [!IMPORTANT]  
>
>- **No cambies el nombre de los archivos (`main.cpp`).**  
>- **Asegúrate de hacer `commit` y `push` antes de la fecha límite.**  
>- **Si encuentras errores en el autograder, revisa tu salida y ajústala según los ejemplos dados.**  
>
---
