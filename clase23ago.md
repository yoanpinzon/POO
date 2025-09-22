# Reto 

<div style="display: flex; justify-content: center;">

```mermaid
classDiagram
    class Empleado {
        - string nombre
        - int salario
        + Empleado()
        + Empleado(string nombre, int salario)
        + int calcularSalario()*
        + void mostrarInfo()*
        + string getNombre()
        + void setNombre(string nombre)
        + int getSalario()
        + void setSalario(int salario)
    }

    class Gerente {
        - int bono
        + Gerente(int bono)
        + Gerente(string nombre, int salario, int bono)
        + int calcularSalario()
        + void mostrarInfo()
        + int getBono()
        + void setBono(int bono)
    }

    class Ingeniero {
        - int horasExtra
        - int pagoHoraExtra
        + Ingeniero()
        + Ingeniero(int horasExtra, int pagoHoraExtra)
        + Ingeniero(string nombre, int salario, int horasExtra, int pagoHoraExtra)
        + int calcularSalario()
        + void mostrarInfo()
        + int getHorasExtra()
        + void setHorasExtra(int horasExtra)
        + int getPagoExtra()
        + void setPagoExtra(int pagoExtra)
    }

    class Vendedor {
        - int ventas
        - float comision
        + Vendedor(int ventas, float comision)
        + Vendedor(string nombre, int salario, int ventas, float comision)
        + int calcularSalario()
        + void mostrarInfo()
        + int getVentas()
        + void setVentas(int ventas)
        + int getComision()
        + void setComision(float comision)
    }

    Empleado <|-- Gerente
    Empleado <|-- Ingeniero
    Empleado <|-- Vendedor
```

</div>
