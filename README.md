# 💻 Simpletron Compiler & Simulator

**Proyecto Final: Diseño e Implementación de un Compilador y Máquina Virtual**

---

## 📌 Acerca del Proyecto
Este repositorio alberga la construcción de un sistema de dos piezas fundamentales:
1. **Un Compilador** escrito en `C++` que traduce programas de un lenguaje de alto nivel ("Simple") a Lenguaje de Máquina Simpletron (SML).
2. **Un Simulador** escrito en `C` que actúa como la CPU virtual, capaz de interpretar el código SML generado, ejecutar operaciones aritméticas complejas y gestionar la memoria dinámica.

## 👤 Autor
* **Desarrollador:** [Nombre Completo de tu Compañero]
* **Repositorio oficial:** [https://github.com/aldairpaleta-cpu/Simpletron.git](https://github.com/aldairpaleta-cpu/Simpletron.git)

---

## 🚀 Características Principales
* **Conversión Infija a Postfija:** Uso de pilas (Stacks) para evaluar operaciones aritméticas respetando jerarquías.
* **Manejo de Errores Fatales:** El simulador previene desbordamientos de memoria (Overflow), saltos fuera de rango y división/módulo por cero.
* **Nuevas Instrucciones SML:**
  * `34`: Operación de Módulo (`%`).
  * `35`: Operación de Exponenciación (`^`).
* **Volcado de Memoria (Memory Dump):** Registro exacto del estado de los acumuladores, contadores y las 100 posiciones de memoria tras la ejecución.

---

## ⚙️ Instrucciones de Instalación y Uso

### 1. Compilación
Abre la terminal en la raíz del proyecto y ejecuta:

```bash
# Compilar la máquina virtual
gcc -o simpletron.exe simpletron.c

# Compilar el traductor
g++ -o compilador.exe compilador.cpp