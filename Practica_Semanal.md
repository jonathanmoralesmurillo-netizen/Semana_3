| <div align="right"><img src="../../Logo-UNA-Rojo_FondoTransparente%20(2).png" width="120" alt="Logo UNA" /></div> | | <p align="right"><img src="../../images.jpeg" width="120" alt="Logo EscINF" /></p> |
|:----------------------------------------------------|:-------------------------------------------------------------:|------------------------------------------------------------:|

**Programa de curso** · **Programación II**  
**Carrera:** Ingeniería de Sistemas de Información con grado en Bachillerato y salida lateral de Diplomado en Programación de Aplicaciones Informáticas.

---

# Semana 3 – Práctica semanal

**Contenidos:** Patrón Delegate, Manejo de excepciones.

---

## Actividad 1 (Delegate)

- Implemente `Impresora` que delegue en `IDispositivoSalida` (interfaz con `void escribir(const std::string&)`).
- Incluya dos implementaciones: `Consola` y `Archivo` (escribe en un archivo de texto).
- En `main`, cree una impresora que use primero consola y luego cambie a archivo; imprima el mismo mensaje en ambos.

---

## Actividad 2 (Excepciones)

- Implemente `divisionSegura(double a, double b)` que lance una excepción derivada de `std::exception` si `b == 0`.
- En `main`, llame con valores válidos e inválidos y capture la excepción mostrando el mensaje. Documente en MD por qué se captura por referencia `const`.

---

## Actividad 3 (RAII y excepciones)

- Cree una clase `Buffer` que en el constructor reserve un array de N caracteres y en el destructor lo libere.
- Simule un constructor que a veces lanza (por ejemplo, si N <= 0). Verifique que no hay fuga si se lanza. Explique en MD la relación con RAII.

---

**Formato de entrega:** Código y explicaciones en **archivo(s) MD (Markdown)**.
