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
