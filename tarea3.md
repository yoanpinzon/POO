# **🧮 Tarea 3 - Sistema de Nómina en C++**

[![Unirse a la tarea](https://img.shields.io/badge/%F0%9F%91%89%20Unirse%20a%20la%20tarea%20en%20GitHub%20Classroom-blue?style=for-the-badge)](https://classroom.github.com/a/KxW3VjAg)

## **📢🚨 FECHA LÍMITE: Lunes 29 de septiembre - 10:00am 🚨📢** <!-- omit in toc -->

⚠️ **ENTREGAS FUERA DE TIEMPO NO SERÁN ACEPTADAS.**  
✅ **Haz `commit` y `push` antes del plazo y verifica tu entrega en GitHub Classroom.**

---

## **📖 Descripción de la Tarea** <!-- omit in toc -->

Vas a desarrollar un **Sistema de Nómina en C++** interactivo, que permita gestionar empleados de distintos tipos (`Ingeniero`, `Gerente`, `Vendedor`, `Repartidor`) mediante **comandos en consola**.

El programa debe:

* Registrar empleados mediante comandos de tipo `AGREGAR`.
* Calcular su salario usando **polimorfismo**.
* Mostrar información detallada de cada empleado.
* Calcular y mostrar el **total de la nómina**.

Se trabajará con **clases, herencia, métodos virtuales y vectores de punteros**.

Se provee un código base, y tu objetivo es completar las funcionalidades faltantes y manejar correctamente casos especiales, asegurándote de que cada clase tenga un archivo .h para la declaración y un archivo .cpp separado para la implementación.

> ⚠️ **Importante:** La fecha límite es **lunes 29 de septiembre a las 10:00am**.


## **📌 Comandos del Programa**

1️⃣ **SALARIO\_MINIMO** `<valor>`

* Define el **salario mínimo** que se aplicará a todos los empleados.
* Todos los salarios calculados por `calcularSalario()` deben ajustarse si son menores que este valor.
* **Valor por defecto:** Si no se define, el salario mínimo será **1000**.

Ejemplo:

```text
SALARIO_MINIMO 1000
```

2️⃣ **AGREGAR** `<TipoEmpleado>` `<Nombre>` `<SalarioBase>` `[otros atributos]`

* Agrega un empleado al sistema.

* Tipos de empleado y atributos adicionales:

  * `Ingeniero`: `<HorasExtras>` `<ValorHoraExtra>`
  * `Gerente`: `<Bono>`
  * `Vendedor`: `<TotalVentas>` `<Comision>`
  * `Repartidor`: `<HorasTrabajadas>` `<PagoPorHora>` *(no utiliza salario base)*

* Ejemplos:

```text
AGREGAR Ingeniero Alice 1200 15 20
AGREGAR Gerente Bob 2000 500
AGREGAR Vendedor Charlie 1000 3000 0.10
AGREGAR Repartidor David 40 15
```

3️⃣ **MOSTRAR**

* Muestra información de todos los empleados registrados.

4️⃣ **NOMINA**

* Muestra el **total de la nómina**, sumando los salarios de todos los empleados:

```text
Total a pagar en nomina: 5300
```

5️⃣ **SALIR**

* Termina la ejecución del programa.

---

## **📌 Casos especiales a tener en cuenta**

1. **Horas extras máximas para Ingenieros:**

   * Un ingeniero no puede registrar más de **50 horas extras**. Si se intenta agregar un valor mayor, se ajusta automáticamente a 50.

2. **Bono colectivo para vendedores:**

   * Si la suma total de ventas de todos los vendedores supera 1,000,000, cada vendedor recibe un bono extra equivalente al 2% del total combinado de ventas de todos los vendedores

3. **Validaciones de comisión de vendedores:**

   * La comisión debe estar entre **0 y 1**. Valores fuera de este rango se ajustan automáticamente.

4. **Salario mínimo:**

   * Ningún empleado puede tener un salario total menor al mínimo definido. (por ejemplo 1000).

> ⚠️ Estas reglas deben implementarse dentro del cálculo de salario y reflejarse correctamente al usar los comandos `MOSTRAR` y `NOMINA`.


## **📌 Casos de prueba**

### Caso 1 

**Entrada:**

```
SALARIO_MINIMO 1000
AGREGAR Ingeniero Alice 1200 15 20
AGREGAR Gerente Bob 2000 500
AGREGAR Vendedor Charlie 1000 3000 0.10
MOSTRAR
NOMINA
SALIR
```

**Salida esperada:**

```
[Ingeniero] Alice | Base: 1200 | Horas extras: 15 | Valor extra: 20 | Total: 1500
[Gerente] Bob | Base: 2000 | Bono: 500 | Total: 2500
[Vendedor] Charlie | Base: 1000 | Ventas: 3000 | Comision: 0.1 | Total: 1300
Total a pagar en nomina: 5300
```

---

### Caso 2 

**Entrada:**

```
AGREGAR Gerente Alice 3000 500
AGREGAR Gerente Bob 2500 400
AGREGAR Ingeniero Carol 2000 10 20
AGREGAR Ingeniero David 1800 5 15
AGREGAR Vendedor Eve 1000 50000 0.05
AGREGAR Vendedor Frank 1200 40000 0.04
AGREGAR Repartidor Grace 140 20
AGREGAR Repartidor Heidi 130 25
AGREGAR Ingeniero Ivan 1500 20 10
AGREGAR Vendedor Judy 1000 30000 0.03
NOMINA
SALARIO_MINIMO 1000
AGREGAR Vendedor Robert 500 500 0.1
MOSTRAR
NOMINA
SALIR
```

**Salida esperada:**

```
Total a pagar en nomina: 26425
[Gerente] Alice | Base: 3000 | Bono: 500 | Total: 3500
[Gerente] Bob | Base: 2500 | Bono: 400 | Total: 2900
[Ingeniero] Carol | Base: 2000 | Horas extras: 10 | Valor extra: 20 | Total: 2200
[Ingeniero] David | Base: 1800 | Horas extras: 5 | Valor extra: 15 | Total: 1875
[Vendedor] Eve | Base: 1000 | Ventas: 50000 | Comision: 0.05 | Total: 3500
[Vendedor] Frank | Base: 1200 | Ventas: 40000 | Comision: 0.04 | Total: 2800
[Repartidor] Grace | Horas trabajadas: 140 | Pago por hora: 20 | Total: 2800
[Repartidor] Heidi | Horas trabajadas: 130 | Pago por hora: 25 | Total: 3250
[Ingeniero] Ivan | Base: 1500 | Horas extras: 20 | Valor extra: 10 | Total: 1700
[Vendedor] Judy | Base: 1000 | Ventas: 30000 | Comision: 0.03 | Total: 1900
[Vendedor] Robert | Base: 500 | Ventas: 500 | Comision: 0.1 | Total: 1000
Total a pagar en nomina: 27425
```

---

## **📌 ¿Cómo entregar la tarea en GitHub Classroom?** <!-- omit in toc -->

### **📝 Pasos para entregar tu código correctamente:** <!-- omit in toc -->

## 1️⃣ Aceptar la tarea  <!-- omit in toc -->
1. **Accede al enlace de la tarea.
2. **Haz clic en "Aceptar la tarea"** para que se genere un repositorio en GitHub automáticamente.
3. Una vez aceptada, **se habrá creado un repositorio en GitHub** con la siguiente dirección (reemplaza `TU_USUARIO` con tu nombre de usuario en GitHub):  
   ```
   https://github.com/profesorcito/tarea3-TU_USUARIO
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
   git clone https://github.com/profesorcito/tarea3-TU_USUARIO.git
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


