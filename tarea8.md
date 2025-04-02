# **🧮 Tarea 8 - Tarea Final**

## **📢🚨 FECHA LÍMITE: Lunes 7 de abril - 23:59 🚨📢** <!-- omit in toc -->

⚠️ **ENTREGAS FUERA DE TIEMPO NO SERÁN ACEPTADAS.**  
✅ **Haz `commit` y `push` antes del plazo y verifica tu entrega en GitHub Classroom.**

---

## **📖 Descripción de la Tarea** <!-- omit in toc -->

En este proyecto, implementarás un sistema de gestión bancaria en **C++** aplicando los conceptos de **composición y herencia** en la relación entre clases. El programa permitirá al usuario administrar un banco, manejando clientes y cuentas bancarias. El propósito principal es que aprendas a implementar y manipular clases que contienen otras clases como atributos, consolidando así tus conocimientos sobre **composición en programación orientada a objetos (POO)**. Además, el sistema deberá incluir **persistencia de datos** mediante la **serialización en formato JSON**, permitiendo que la información del banco sea almacenada y recuperada desde un archivo externo.

---

### **Enunciado del Problema**  

El **Banco Javeriano** desea desarrollar un sistema en **C++** que gestione información de clientes y cuentas bancarias. El sistema debe cumplir con los siguientes requisitos:  

1. **Banco**:  
   - Debe tener un nombre y almacenar clientes y cuentas en vectores.  
   - Permitir la adición de nuevos clientes y cuentas.  
   - Mostrar la lista de clientes y cuentas.  
   - Guardar y cargar los datos en un archivo **JSON**.  

2. **Clientes**:  
   - Cada cliente tiene un **ID único** (asignado automáticamente comenzando en 1), un **nombre** y una **dirección**.  

3. **Cuentas**:  
   - Cada cuenta tiene un **número único** (asignado automáticamente comenzando en 100), un **saldo** y está asociada a un **cliente**.  
   - Existen dos tipos de cuentas mediante **herencia**:  
     - **Cuenta de Ahorros**: Tiene una **tasa de interés**, la cual se aplica de manera mensual al saldo disponible en la cuenta.  
     - **Cuenta Corriente**: Tiene un **límite de sobregiro**, lo que permite al cliente retirar más dinero del que posee en su saldo, hasta un monto límite definido.  

4. **Funcionalidad del sistema**:  
   - Agregar clientes y cuentas.  
   - Mostrar clientes y cuentas.  
   - Guardar y cargar datos desde un archivo **BancoJaveriano.json** mediante **serialización en JSON**.  
   - Mostrar estadísticas del banco, incluyendo:  
     - Total de clientes registrados.  
     - Total de cuentas registradas.  
     - Promedio del saldo de las cuentas.  
     - Número de cuentas de ahorro y cuentas corrientes.  
   - Aplicar la **tasa de interés** a todas las cuentas de ahorro.  

---

### **Menú Principal**  

Cuando se ejecute el programa, debe mostrarse el siguiente menú interactivo:  

```
MENU BANCO JAVERIANO
1) MANTENIMIENTO DE CLIENTES
   1.1) Agregar Cliente
   1.2) Listar Clientes

2) MANTENIMIENTO DE CUENTAS
   2.1) Agregar Cuenta
   2.2) Listar Cuentas

3) ESTADÍSTICAS
   3.1) Total de Clientes
   3.2) Total de Cuentas
   3.3) Promedio del Saldo de las Cuentas
   3.4) Número de Cuentas de Ahorro
   3.5) Número de Cuentas Corrientes

4) OPERACIONES FINANCIERAS
   4.1) Aplicar Tasa de Interés a Cuentas de Ahorro
   4.2) Consignar Dinero en una Cuenta
   4.3) Retirar Dinero de una Cuenta
5) SALIR
   5.1) Guardar los datos en BancoJaveriano.json y cerrar el programa.
```


