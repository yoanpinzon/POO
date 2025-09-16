# **🧮 Tarea 2 - Sistema de Facturación Avanzado**

## **📢🚨 FECHA LÍMITE: Lunes 22 de septiembre - 10:00am 🚨📢** <!-- omit in toc -->

⚠️ **ENTREGAS FUERA DE TIEMPO NO SERÁN ACEPTADAS.**  
✅ **Haz `commit` y `push` antes del plazo y verifica tu entrega en GitHub Classroom.**

---

## **📖 Descripción de la Tarea** <!-- omit in toc -->

En esta tarea, vas a desarrollar un **Sistema de Facturación Avanzado en C++**. 💻🛍️
El programa permitirá:

* Gestionar un **inventario de productos**.
* Registrar **ventas**.
* Aplicar **promociones combinadas**.
* Generar **facturas** automáticamente.


Esta actividad refuerza conceptos de **C++** como:

* Clases y objetos
* Encapsulación
* Vectores y estructuras de datos
* Métodos y sobrecarga de operadores
* Entrada y salida de datos

Se provee un **código base**, y tu objetivo es **completar las funcionalidades faltantes** y manejar correctamente **casos especiales**.

> ⚠️ **Importante:** La fecha límite es **lunes 22 de septiembre a las 10:00am**.

¡Manos a la obra y mucho éxito! 💪💻

## **📌 Objetivos del sistema**

1. Crear un sistema modular con las clases: `Producto`, `Inventario`, y `Factura`.
2. Gestionar un inventario **dinámico** (agregar, eliminar, actualizar productos).
3. Registrar ventas y aplicar promociones combinadas.
4. Calcular totales y generar facturas automáticamente.
5. Permitir **casos básicos** (sin promociones) y **casos avanzados** (promociones y descuentos).

---

## **📌 Comandos del Programa**

El programa debe soportar los siguientes comandos:

1️⃣ **AGREGAR** `<nombre>` `<cantidad>` `<precio>`

* Agrega un producto al inventario.
* Si el producto ya existe, suma la nueva cantidad al stock y **actualiza el precio si es diferente**, mostrando un mensaje especial.

2️⃣ **ELIMINAR** `<nombre>`

* Elimina un producto del inventario.
* Si el producto no existe, muestra un mensaje de error.

3️⃣ **BUSCAR** `<nombre>`

* Muestra la cantidad y el precio actual del producto.
* Si no existe, muestra un mensaje de error.

4️⃣ **VENDER** `<nombre>` `<cantidad>`

* Registra una venta y reduce el stock del inventario.
* Si la cantidad solicitada es mayor al stock disponible, vende **solo lo que haya** y muestra un mensaje indicando la cantidad vendida.
* Cada venta se registra en la factura, separando por precio actual si el producto tuvo actualizaciones de precio.

5️⃣ **FACTURAR**

* Muestra todos los productos vendidos y el total a pagar.
* Aplica promociones combinadas si se cumplen las condiciones (ambos productos en la factura).
* Una vez facturado, **la factura se limpia**.

6️⃣ **PROMO\_COMBINADA** `<producto1>` `<producto2>` `<descuento>`

* Define una promoción que aplica un descuento si ambos productos se venden juntos.
* Si la promoción ya existe para los mismos productos, se muestra un mensaje indicando que ya existe y **no se duplica**.

7️⃣ **STOCK\_BAJO**

* Lista todos los productos con stock menor a 5 unidades.

8️⃣ **INVENTARIO**

* Muestra el inventario actual calculando el **valor total** de todos los productos (stock × precio).
* No modifica el inventario ni la factura.

9️⃣ **SALIR**

* Finaliza el programa de manera segura.

---

## **📌 Comportamientos especiales / reglas importantes**

* **Actualizar precio al agregar:**
  Si un producto agregado ya existe pero con un precio diferente, se debe actualizar el precio y notificar:

  ```
  [Precio <Producto> actualizado]
  ```

* **Venta con stock insuficiente:**
  Si se intenta vender más de lo disponible, se vende solo lo que hay y se notifica:

  ```
  Stock insuficiente para <Producto>. Solo se venderá <CantidadDisponible>
  ```

* **Registro de ventas:**
  Cada venta se guarda en la factura. Si un producto se vende con diferentes precios en distintas transacciones, se **registran por separado** según el precio de venta.

* **Promociones combinadas:**

  * Se aplican solo si ambos productos están presentes en la factura.
  * Cada promoción se aplica **una sola vez**, sin importar la cantidad de productos.
  * No se pueden duplicar promociones para la misma combinación de productos; si se intenta, se muestra:

    ```
    Promo <Producto1> + <Producto2> ya existe
    ```

* **Facturación y limpieza:**
  Tras ejecutar `FACTURAR`, la lista de ventas se vacía automáticamente para permitir nuevas transacciones.

* **Inventario dinámico:**
  El inventario refleja siempre los cambios de stock y precios, y se puede consultar con `INVENTARIO` (opcional en algunos casos de prueba).

---

Si el usuario ingresa un comando no reconocido, el programa debe mostrar un mensaje de error.

---

## **📌 Casos de prueba**

### Caso 1 - Básico (sin promociones)

#### Entrada

```
AGREGAR Pan 10 500
AGREGAR Leche 20 1500
VENDER Pan 3
VENDER Leche 5
FACTURAR
SALIR
```

#### Salida esperada

```
[Pan, 10, 500]
[Leche, 20, 1500]
[Pan, 7, 500]
[Leche, 15, 1500]
Total: 9000
```

---

### Caso 2 - Intermedio (permite actualizar el precio)

#### Entrada

```
AGREGAR Pan 10 500
AGREGAR Leche 20 1500
AGREGAR Mantequilla 5 2000
VENDER Pan 8
VENDER Leche 10
AGREGAR Pan 8 500
AGREGAR Leche 10 1200
VENDER Pan 5
VENDER Leche 3
FACTURAR
SALIR
```

#### Salida esperada

```
[Pan, 10, 500]
[Leche, 20, 1500]
[Mantequilla, 5, 2000]
[Pan, 2, 500]
[Leche, 10, 1500]
[Pan, 10, 500]
[Leche, 20, 1200]
[Precio Leche actualizado]
[Pan, 5, 500]
[Leche, 17, 1200]
Total: 25100
```

### Caso 3 - Avanzado (permite promo)

#### Entrada

```
AGREGAR Pan 10 500
AGREGAR Leche 20 1500
AGREGAR Mantequilla 5 2000
AGREGAR Jugo 15 1200
AGREGAR Queso 8 2500
INVENTARIO
VENDER Queso 3
VENDER Jugo 1
PROMO_COMBINADA Pan Leche 200
PROMO_COMBINADA Queso Jugo 150
AGREGAR Pan 10 499
PROMO_COMBINADA Leche Pan 300
VENDER Pan 3
VENDER Leche 5
VENDER Mantequilla 2
AGREGAR Pan 5 450
AGREGAR Queso 2 2200
VENDER Pan 4
VENDER Queso 3
FACTURAR
INVENTARIO
SALIR
```

#### Salida esperada

```
[Pan, 10, 500]
[Leche, 20, 1500]
[Mantequilla, 5, 2000]
[Jugo, 15, 1200]
[Queso, 8, 2500]
Inventario: 83000
[Queso, 5, 2500]
[Jugo, 14, 1200]
[Pan, 20, 499]
[Precio Pan actualizado]
Promo Leche + Pan ya existe
[Pan, 17, 499]
[Leche, 15, 1500]
[Mantequilla, 3, 2000]
[Pan, 22, 450]
[Precio Pan actualizado]
[Queso, 7, 2200]
[Precio Queso actualizado]
[Pan, 18, 450]
[Queso, 4, 2200]
[Pan+Leche promo aplicada: -300]
[Queso+Jugo promo aplicada: -150]
Total: 29647
Inventario: 62200
```

> Nota: El descuento de la promoción se aplica una sola vez por conjunto.

---

### **📜 Código Base** <!-- omit in toc -->
El siguiente código base debe usarse para resolver este problema.  
⚠️ **No se debe cambiar el nombre de los archivos.**  
- `main.cpp`: Archivo principal del programa.  

#### 📝 `main.cpp`
```cpp
#include <iostream>
#include <vector>
#include <string>

using namespace std;

class Producto {
private:
    string nombre;
    int stock;
    int precio;

public:
    Producto() : nombre("N/A"), stock(0), precio(0) {}
    Producto(string n, int s, int p) : nombre(n), stock(s), precio(p) {}

    string getNombre() const { return nombre; }
    int getStock() const { return stock; }
    int getPrecio() const { return precio; }

    void sumarStock(int s) { stock += s; }
    void venderStock(int s) { stock -= s; }
    void setPrecio(int p) { precio = p; }
};

class Promo {
public:
    string producto1;
    string producto2;
    int descuento;

    // TODO: Implementar los constructores de PROMO
};

int main() {
    vector<Producto> inventario;
    vector<Producto> factura;
    vector<Promo> promociones;

    string comando;

    while (true) {
        cin >> comando;

        if (comando == "AGREGAR") {
            string nom;
            int cant, precio;
            cin >> nom >> cant >> precio;

            // TODO: Implementar la solución para agregar
        }
        else if (comando == "VENDER") {
            string nom;
            int cant;
            cin >> nom >> cant;
            // TODO: Implementar la solución para vender
        }
        else if (comando == "PROMO_COMBINADA") {
            string p1, p2;
            int desc;
            cin >> p1 >> p2 >> desc;
            // TODO: Implementar la solución para promo
        }
        else if (comando == "FACTURAR") {
            int total = 0;

            // TODO: Implementar la solución para facturar

            cout << "Total: " << total << endl;
        }
        else if (comando == "INVENTARIO") {
            int totalInventario = 0;

            // TODO: Implementar la solución para inventario

            cout << "Inventario: " << totalInventario << endl;
        }

        else if (comando == "SALIR") {
            break;
        }

        else {
            cout << "ERROR" << endl;
        }
    }

    return 0;
}
```

## **📌 ¿Cómo entregar la tarea en GitHub Classroom?** <!-- omit in toc -->

### **📝 Pasos para entregar tu código correctamente:** <!-- omit in toc -->

## 1️⃣ Aceptar la tarea  <!-- omit in toc -->
1. **Accede al enlace de la tarea.
2. **Haz clic en "Aceptar la tarea"** para que se genere un repositorio en GitHub automáticamente.
3. Una vez aceptada, **se habrá creado un repositorio en GitHub** con la siguiente dirección (reemplaza `TU_USUARIO` con tu nombre de usuario en GitHub):  
   ```
   https://github.com/profesorcito/tarea2-TU_USUARIO
   ```
4. Verifica que el repositorio esté disponible en tu cuenta de GitHub.  

## 2️⃣ Clonar el repositorio en tu computadora <!-- omit in toc -->  
5. **Abre una terminal o Git Bash** en tu computadora.  
6. **Ubícate en la carpeta donde deseas guardar el proyecto** con el siguiente comando (puedes cambiar la ruta según tu preferencia):  
   ```bash
   cd ~/Desktop/CLionProjects
   ```
7. **Clona tu repositorio** con el siguiente comando (reemplaza `TU_USUARIO` con tu usuario en GitHub):  
   ```bash
   git clone https://github.com/profesorcito/tarea2-TU_USUARIO.git
   ```

## 3️⃣ Abrir el proyecto en CLion <!-- omit in toc -->  
8. **Abre CLion y carga el proyecto:**  
   - Presiona `Alt + F`.  
   - Selecciona **New** → **Project**.  
   - En la parte izquierda, selecciona **C++ Executable**.  
   - Busca la carpeta donde quedó el repositorio dentro de `CLionProjects`.  
   - Debe llamarse:  
     ```
     tarea2-TU_USUARIO
     ```
   - Haz clic en **Create**.  
   - Si aparece un mensaje preguntando si deseas confiar en el proyecto, selecciona **Yes**.  

## 4️⃣ Modificar y probar el código <!-- omit in toc -->  
9. **Edita y prueba el código:**  
   - Abre `main.cpp` y escribe el código necesario.  
   - Ejecuta el programa y verifica que la salida sea la esperada.  
   - Realiza pruebas para asegurarte de que todo funcione correctamente.  

## 5️⃣ Guardar y subir los cambios a GitHub <!-- omit in toc -->  
10. **Guarda los cambios y súbelos a GitHub** con los siguientes comandos en la terminal dentro de la carpeta del repositorio:  
   ```bash
   git add .
   git commit -m "Intento 1"
   git push
   ```
   
> [!WARNING]  
> Si el comando `git push` falla debido a cambios en el repositorio remoto, primero ejecuta `git pull` para sincronizar los cambios y luego vuelve a intentar con `git push`.

## 6️⃣ Verificar la entrega en GitHub Classroom <!-- omit in toc -->  
11. **Revisa en GitHub si tu tarea fue subida correctamente:**  
   - Ingresa a tu repositorio en GitHub.
   - Verifica que los archivos y cambios estén reflejados.  
12. **Revisa la pestaña "Actions" en GitHub:**  
   - Si la tarea fue aceptada, se mostrará un ícono verde ✅.  
   - Si hubo errores, se mostrará un ícono rojo ❌.  
   - Haz clic en el commit más reciente y revisa **"run-autograding-test"** para ver los detalles.  
13. **Corrige los errores y sube los cambios nuevamente** hasta que la evaluación esté en verde.

---
> [!IMPORTANT]  
>- **No cambies el nombre de los archivos (`main.cpp`).**  
>- **Asegúrate de hacer `commit` y `push` antes de la fecha límite.**  
>- **Si encuentras errores en el autograder, revisa la salida y ajústala según los ejemplos dados.**  
>


