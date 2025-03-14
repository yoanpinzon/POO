
# **🧮 Tarea 2 - Reto C++**

[![Unirse a la tarea](https://img.shields.io/badge/%F0%9F%91%89%20Unirse%20a%20la%20tarea%20en%20GitHub%20Classroom-blue?style=for-the-badge)](https://classroom.github.com/a/sHyJsgJf)


## **📢🚨 FECHA LÍMITE: Lunes 17 de febrero - 11:59 PM 🚨📢** <!-- omit in toc -->

⚠️ **ENTREGAS FUERA DE TIEMPO NO SERÁN ACEPTADAS.**  
✅ **Haz `commit` y `push` antes del plazo y verifica tu entrega en GitHub Classroom.**

---

## **📖 Descripción de la Tarea** <!-- omit in toc -->

La tarea consta de **dos problemas** con distinta dificultad y puntaje asignado.

---

## **📌 Problema 1 (40 puntos)** <!-- omit in toc -->

### **Descripción** <!-- omit in toc -->

ONE OK ROCK comenzó su carrera tocando en pequeños clubes y avanzó hasta presentarse en estadios internacionales. Imagina que cada concierto representa un número en su trayectoria, desde el primero hasta el más reciente. Su crecimiento ha sido una historia de esfuerzo y perseverancia, enfrentando desafíos y superando barreras culturales para llegar a audiencias de todo el mundo. Tu tarea es escribir un programa que reciba un número entero positivo **N**, representando la cantidad de conciertos, e imprima en líneas separadas los números del **1** al **N**, simbolizando cada presentación de la banda. Este proceso reflejará la progresión de ONE OK ROCK desde sus humildes inicios hasta sus grandes actuaciones en escenarios internacionales.

Además, puedes imaginar que cada número representa un hito importante en la carrera de la banda, como el lanzamiento de un álbum exitoso, una colaboración destacada o una actuación inolvidable en un festival de renombre.

### **📌 Entrada** <!-- omit in toc -->

- Un solo número entero **N** *(1 ≤ N ≤ 10000)*.

### **📌 Salida** <!-- omit in toc -->

- **N** líneas, cada una con un número del **1** al **N**, representando cada concierto de ONE OK ROCK en su camino al éxito.

### **Ejemplo de Entrada y Salida** <!-- omit in toc -->

### **Ejemplo 1** <!-- omit in toc -->

#### Entrada: <!-- omit in toc -->

```
3
```

#### Salida: <!-- omit in toc -->

```
1
2
3

```

### **Ejemplo 2** <!-- omit in toc -->

#### Entrada: <!-- omit in toc -->

```
7
```

#### Salida: <!-- omit in toc -->

```
1
2
3
4
5
6
7

```

### **📜 Código Base** <!-- omit in toc -->
El siguiente código base debe usarse para resolver este problema.  
⚠️ **No se debe cambiar el nombre del archivo, debe llamarse `punto1.cpp`.**  

```cpp
#include <iostream>

using namespace std;

int main() {
    int n; // Variable para alamacenar la entrada del usuario
    cin >> n; // Lectura de la entrada desde la consola

    // TODO: Implementar la solución para el problema correspondiente

    return 0; // Indica que el programa finalizó correctamente
}
```

---

## **📌 Problema 2 (60 puntos)**  <!-- omit in toc -->

### **📖 Historia**  <!-- omit in toc -->

En una remota academia de criptografía, los estudiantes han descubierto una secuencia numérica con propiedades desconocidas. Se dice que esta serie fue utilizada por una antigua civilización para cifrar mensajes ocultos en textos religiosos y científicos. Sin embargo, los manuscritos solo revelan los primeros dos números y el número total de términos necesarios.  

Tu misión es recrear la secuencia y revelar el número clave que usaban para verificar la autenticidad de los mensajes. Dependiendo de la estructura del mensaje, el número clave podría cambiar su interpretación.  

Los registros indican que esta civilización estableció un límite en la cantidad de términos que podían generarse. **Solo se permitía calcular hasta N = 29**, ya que creían que los números primos eran esenciales en su sistema, y **29 es el mayor número primo menor a 30**. Cualquier cálculo fuera de este rango era considerado inexacto o incluso prohibido en su método de análisis.  

---

### **📜 Reglas de la Serie**  <!-- omit in toc -->

1. Se reciben tres números enteros: **A, B, N**.  
   - **A** y **B** → Son los dos primeros términos de la serie.  
   - **N** → Indica cuántos términos debe generar el sistema.  
2. Cada término de la serie se calcula como la **suma de los dos anteriores**.  
3. El resultado esperado es el **último dígito** del término final.  

### **🎯 Condición Especial**  <!-- omit in toc -->

Las investigaciones sugieren que cuando **N** es un número primo, los antiguos matemáticos no utilizaban el último dígito, sino el **primer dígito** del término final, ya que creían que los números primos tenían propiedades divinas y eran la clave de su código numérico.  

---

## **📌 Entrada**  <!-- omit in toc -->

El programa recibirá **una única línea de entrada** con tres números enteros separados por un espacio:  

- **A** *(1 ≤ A ≤ 10,000)* → Primer número de la serie.  
- **B** *(1 ≤ B ≤ 10,000)* → Segundo número de la serie.  
- **N** *(1 ≤ N ≤ 29)* → Cantidad de términos a generar (limitado por razones estructurales).  

---

## **📌 Salida**  <!-- omit in toc -->

El programa debe imprimir **un único número**:  

- El **último dígito** del término final generado, salvo cuando **N** sea primo, en cuyo caso se imprimirá el **primer dígito**.  

---

### **Ejemplos de Entrada y Salida**  <!-- omit in toc -->

#### **Ejemplo 1** (**N** no es primo)  <!-- omit in toc -->

##### Entrada:  <!-- omit in toc -->
```
1 1 12
```  

##### Salida:  <!-- omit in toc -->
```
4
```  

*(Serie generada: 1 1 2 3 5 8 13 21 34 55 89 144 → Último dígito: 4)*  

---

#### **Ejemplo 2** (**N** es primo) <!-- omit in toc -->  

##### Entrada:  <!-- omit in toc -->
```
130 5 13
```  

##### Salida:  <!-- omit in toc -->
```
1
```  

*(Serie generada: 130 5 135 140 275 415 690 1105 1795 2900 4695 7595 12290 → Primer dígito: 1)*  

---

## **📜 Notas Importantes**  <!-- omit in toc -->

- **El sistema debe manejar números grandes sin desbordarse.**  
- **Se debe optimizar la generación de la serie para evitar un uso excesivo de memoria.**  

---

### **📜 Código Base** <!-- omit in toc -->
El siguiente código base debe usarse para resolver este problema.  
⚠️ **No se debe cambiar el nombre del archivo, debe llamarse `punto2.cpp`.**  

```cpp
#include <iostream>

using namespace std;

// Función para determinar si un número es primo
bool esPrimo(int n) {
    if (n < 2) return false;
    for (int i = 2; i * i <= n; i++) {
        if (n % i == 0) return false;
    }
    return true;
}

// Función para obtener el primer dígito de un número
int primerDigito(int num) {
    // TODO: Implementar la extracción del primer dígito del número
    return 0;
}

// Función para calcular el último dígito del término final de la serie
int calcularUltimoDigito(int a, int b, int n) {
    // TODO: Implementar la generación de la serie y extraer el dígito correspondiente
    return 0;
}

int main() {
    int a, b, n;
    cin >> a >> b >> n; // Lectura de los valores de entrada
    cout << calcularUltimoDigito(a, b, n) << endl; // Cálculo e impresión del resultado
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
   https://github.com/profesorcito/tarea-2-TU_USUARIO
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
   git clone https://github.com/profesorcito/tarea-2-TU_USUARIO.git
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
     tarea-2-TU_USUARIO
     ```
   - Haz clic en **Create**.  

> [!IMPORTANT]
>
> Aparecerá un mensaje preguntando si deseas crear el proyecto sobre los archivos existentes. **Debes aceptar.**  Si pregunta si quieres abrirlo en esta ventana, **también acepta.**  
>

## 4️⃣ Modificar y probar el código <!-- omit in toc --> 
8. **Editar y ejecutar `punto1.cpp`:**  
   - Busca `punto1.cpp` y ábrelo.  
   - Escribe el código necesario para resolver el problema.  
   - Antes de compilar, en la parte superior, en el menú desplegable junto al botón **Build** (🔨), **selecciona `punto1`**.  
   - Ejecuta el programa y verifica que la salida sea la esperada.  

9. **Editar y ejecutar `punto2.cpp`:**  
   - Busca `punto2.cpp` y ábrelo.  
   - Escribe el código necesario para resolver el problema.  
   - Antes de compilar, en la parte superior, en el menú desplegable junto al botón **Build** (🔨), **selecciona `punto2`**.  
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
>- **No cambies el nombre de los archivos (`punto1.cpp` y `punto2.cpp`).**  
>- **Asegúrate de hacer `commit` y `push` antes de la fecha límite.**  
>- **Si encuentras errores en el autograder, revisa tu salida y ajústala según los ejemplos dados.**  
>
---


