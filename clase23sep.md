# Reto 

<div style="display: flex; justify-content: center;">

```mermaid
classDiagram
    class Empleado {
        # string nombre
        # int salarioBase
        + Empleado()
        + Empleado(string nombre, int salarioBase)
        + int calcularSalario()*
        + void mostrarInfo()*
        + string getNombre()
        + void setNombre(string nombre)
        + int getSalarioBase()
        + void setSalarioBase(int salarioBase)
    }

    class Gerente {
        - int bono
        + Gerente()
        + Gerente(string nombre, int salarioBase, int bono)
        + int calcularSalario()
        + void mostrarInfo()
        + int getBono()
        + void setBono(int bono)
    }

    class Ingeniero {
        - int horasExtras
        - int valorHoraExtra
        + Ingeniero()
        + Ingeniero(int horasExtras, int valorHoraExtra)
        + Ingeniero(string nombre, int salarioBase, int horasExtras, int valorHoraExtra)
        + int calcularSalario()
        + void mostrarInfo()
        + int getHorasExtras()
        + void setHorasExtras(int horasExtras)
        + int getValorHoraExtra()
        + void setValorHoraExtra(int valorHoraExtra)
    }

    class Vendedor {
        - int totalVentas
        - float comision
        + Vendedor()
        + Vendedor(int totalVentas, float comision)
        + Vendedor(string nombre, int salarioBase, int totalVentas, float comision)
        + int calcularSalario()
        + void mostrarInfo()
        + int getTotalVentas()
        + void setTotalVentas(int totalVentas)
        + float getComision()
        + void setComision(float comision)
    }

    Empleado <|-- Ingeniero
    Empleado <|-- Gerente
    Empleado <|-- Vendedor
```
</div>

---

<p>

```text
# Salida esperda 

=== Nomina de empleados ===
[Ingeniero] Alice | Base: 1200 | Horas extra: 15 | Pago extra: 20 | Total: 1500
[Gerente] Bob | Base: 2000 | Bono: 500 | Total: 2500
[Vendedor] Charlie | Base: 1000 | Ventas: 3000 | Comision: 0.1 | Total: 1300

Total a pagar en nomina: 5300
```

</div>
