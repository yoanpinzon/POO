# **Taller 1 - Mi Banco**

## **📢🚨 FECHA LÍMITE: 2 de SEPTIEMBRE - 9:00 AM 🚨📢**

⚠️ **ENTREGAS FUERA DE TIEMPO NO SERÁN ACEPTADAS.**

---

## **📜 Reglas del Banco**

El sistema debe funcionar como una **aplicación de consola en C++** con el siguiente **menú interactivo**:

```
MENU MI BANCO
1. Agregar cliente
2. Listar clientes
3. Consignar
4. Retirar
5. Transferir
6. Totales
0. Salir
```

### **📌 Funcionalidades obligatorias**

1. **Agregar cliente**

   * Se pide el nombre del cliente y se registra con saldo inicial en **0**.
   * El banco puede manejar hasta **100 clientes**.

2. **Listar clientes**

   * Muestra en pantalla todos los clientes registrados y su saldo actual.

3. **Consignar**

   * Se pide el nombre del cliente.
   * Se ingresa un monto y se suma al saldo del cliente.

4. **Retirar**

   * Se pide el nombre del cliente.
   * Se ingresa un monto y se descuenta del saldo del cliente.

5. **Transferir**

   * Se pide el **nombre del cliente origen** y el **nombre del cliente destino**.
   * Se ingresa un monto.
   * El monto se descuenta del saldo del cliente origen y se suma al saldo del cliente destino.
   * Si el cliente origen no tiene fondos suficientes, debe mostrarse un mensaje de error y no realizar la operación.

6. **Totales**

   * Se calcula la suma de todos los saldos de los clientes del banco y se imprime en pantalla.

7. **Salir**

   * El programa termina.

---

### **📌 Funcionalidad Opcional (para puntos adicionales 🎁)**

* **Historial de transacciones**:
  Cada vez que se haga una **consignación, retiro o transferencia**, se debe guardar un registro con:

  * Tipo de operación (Consignar, Retirar, Transferir).
  * Nombre(s) de los clientes involucrados.
  * Monto de la operación.
  * Nuevo saldo del cliente.

  El historial debe poder mostrarse con una nueva opción en el menú:

  ```
  7. Ver historial
  ```

  ✅ Implementar esta funcionalidad otorga **0,5 puntos adicionales sobre la nota final del taller**.

---

## **📌 Ejemplo de Ejecución**

```
MENU MI BANCO
1. Agregar cliente
2. Listar clientes
3. Consignar
4. Retirar
5. Transferir
6. Totales
0. Salir
opcion: 1
Nombre= Juan

opcion: 1
Nombre= Maria

opcion: 3
Nombre= Juan
Monto a consignar=1000

opcion: 5
Cliente origen= Juan
Cliente destino= Maria
Monto= 500

opcion: 2
Juan 500
Maria 500
```

---

## **📌 Pasos para entregar el taller**

1. **Crea un proyecto en CLion llamado `MiBanco`**.
2. **Escribe tu código en `main.cpp`**.
3. **Verifica que compile y funcione correctamente en tu máquina local**.
4. **Crea un repositorio local en ese directorio** con:

   ```bash
   git init
   ```
5. **Crea un archivo `.gitignore`** para evitar subir archivos innecesarios de CLion.
6. **Crea un repositorio público en tu cuenta de GitHub llamado `MiBanco`**.
7. **Sube tu proyecto a GitHub**:

   ```bash
   git remote add origin https://github.com/TU_USUARIO/MiBanco.git
   git add .
   git commit -m "Taller 1 - Mi Banco"
   git push -u origin master
   ```
8. **Envía un correo a `pinzon@gmail.com` con el link de tu repositorio público en GitHub**.

---

## **📜 Notas**

* **El nombre del proyecto en CLion debe ser `MiBanco`.**
* **El repositorio en GitHub también debe llamarse `MiBanco`.**
* **El código debe compilar y ejecutarse en C++ correctamente.**
* **El repositorio en GitHub debe ser público.**
* **El correo debe enviarse antes de la fecha límite.**
* **La funcionalidad opcional suma hasta +0,5 en la nota final del taller.**

---

