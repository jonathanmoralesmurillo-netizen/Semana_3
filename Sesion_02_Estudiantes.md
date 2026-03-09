| <div align="right"><img src="../Logo-UNA-Rojo_FondoTransparente%20(2).png" width="120" alt="Logo UNA" /></div> | | <p align="right"><img src="../images.jpeg" width="120" alt="Logo EscINF" /></p> |
|:----------------------------------------------------|:-------------------------------------------------------------:|------------------------------------------------------------:|

**Programa de curso** · **Programación II**  
**Carrera:** Ingeniería de Sistemas de Información con grado en Bachillerato y salida lateral de Diplomado en Programación de Aplicaciones Informáticas.

---

# Semana 3 – Sesión 2 (Estudiantes)

**Duración:** 2 horas  
**Tema:** Manejo de excepciones

---

## Explicación (resumen)

- **Excepciones:** `try`, `throw`, `catch`. Use excepciones estándar (`std::exception`, `std::runtime_error`) o derivadas. Capturar por referencia `const`. No lanzar en destructores.
- **RAII:** Recurso adquirido en constructor, liberado en destructor; si el constructor lanza, el destructor no se llama para ese objeto (los miembros sí se destruyen).

---

## Espacio para tu código

### Ejercicio 1: divisionSegura y catch

Función `divisionSegura(double a, double b)` que lance una excepción adecuada si `b == 0`. En `main` capture la excepción y muestre un mensaje.

```cpp
// divisionSegura y main con try/catch

```

### Ejercicio 2: Jerarquía de excepciones

Una clase base de excepción y dos derivadas. Lance cada tipo desde funciones distintas y use varios `catch` para manejarlas por tipo.

```cpp
// Clase base y dos derivadas; lanzar y capturar por tipo

```

### Ejercicio 3: RAII

Clase que en el constructor reserve un recurso (por ejemplo array dinámico) y en el destructor lo libere. En un caso de error en el constructor lance excepción; comente por qué el destructor del objeto no se ejecuta pero no hay fuga si los miembros son objetos automáticos.

```cpp
// Clase con new en constructor y delete en destructor; opcional throw en constructor

```

---

## Criterios de validación (para el profesor)

- [ ] Captura por referencia (const exception&)
- [ ] Uso de `using namespace std;`
