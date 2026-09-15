# EJERCICIOS HTML Y CSS

> Repositorio de ejercicios prácticos para el aprendizaje y aplicación de **HTML5, CSS3 y CSS Grid**.

---

## CONTENIDO

El proyecto está dividido en dos secciones principales:

| Sección                   | Descripción                                                        |
| ------------------------- | ------------------------------------------------------------------ |
| **Ejercicios HTML y CSS** | Prácticas fundamentales de estructura HTML y estilos CSS           |
| **Layouts con Grid**      | Ejercicios enfocados en la creación de layouts utilizando CSS Grid |

---

# 01. EJERCICIOS HTML Y CSS

Esta sección contiene **5 ejercicios** enfocados en practicar la construcción de estructuras HTML y la aplicación de estilos mediante CSS.

Cada ejercicio contiene sus respectivos archivos para separar la estructura HTML de los estilos CSS.

### Ejercicio 1

Práctica inicial de creación de estructuras HTML y aplicación de estilos mediante CSS.

### Ejercicio 2

Ejercicio enfocado en continuar trabajando la estructura HTML y diferentes propiedades de CSS.

### Ejercicio 3

Práctica de organización y presentación de elementos HTML utilizando CSS.

### Ejercicio 4

Ejercicio orientado al manejo de estructuras y estilos mediante CSS.

### Ejercicio 5

Integración de los conocimientos adquiridos en los ejercicios anteriores mediante la combinación de HTML y CSS.

---

# 02. LAYOUTS CON GRID

Sección dedicada al aprendizaje de **CSS Grid**, comenzando con estructuras básicas y avanzando hacia layouts utilizando Grid Areas y diseño responsive.

---

## EJERCICIO 1 — MI PRIMERA GRID

Creación de una cuadrícula de **6 elementos**, distribuidos en 3 columnas y 2 filas.

```text
┌──────┬──────┬──────┐
│  1   │  2   │  3   │
├──────┼──────┼──────┤
│  4   │  5   │  6   │
└──────┴──────┴──────┘
```

### Propiedades utilizadas

```css
display: grid;
grid-template-columns;
gap;
```

### Restricción

No utilizar Flexbox. El objetivo es comprender la estructura básica de **CSS Grid**.

---

## EJERCICIO 2 — CAMBIANDO LA ESTRUCTURA

Se modifica la distribución de los elementos utilizando únicamente:

```css
grid-template-columns;
```

### Estructura A

```text
1  2
3  4
5  6
```

### Estructura B

```text
1  2  3
4  5  6
```

### Estructura C

```text
1  2  3  4
5  6  7  8
```

El objetivo es comprender cómo el número de columnas modifica la distribución automática de los elementos dentro del Grid.

---

## EJERCICIO 3 — DASHBOARD

Creación de un dashboard utilizando CSS Grid.

### Elementos

* Ventas
* Usuarios
* Pedidos
* Productos
* Soporte
* Reportes

### Distribución

```text
┌────────────┬────────────┬────────────┐
│   Ventas   │  Usuarios  │  Pedidos   │
├────────────┼────────────┼────────────┤
│ Productos  │  Soporte   │  Reportes  │
└────────────┴────────────┴────────────┘
```

### Conceptos practicados

```css
display: grid;
grid-template-columns;
gap;
```

Además, se trabaja con:

* Box Model
* Pseudoclase `:hover`
* Organización de elementos mediante Grid

---

## EJERCICIO 4 — TARJETA DESTACADA

Creación de una estructura de tarjetas donde una tarjeta ocupa el espacio correspondiente a **dos columnas**.

```text
┌──────────────────────┬──────────┐
│                      │          │
│      DESTACADA       │  CARD 2  │
│                      │          │
├──────────┬───────────┴──────────┤
│  CARD 3  │       CARD 4         │
└──────────┴──────────────────────┘
```

### Propiedad principal

```css
grid-column: span 2;
```

El objetivo es aprender a controlar la posición y el tamaño de los elementos dentro de una cuadrícula.

---

# 03. EJERCICIOS 5 Y 6 — GRID AREAS Y RESPONSIVE

Los ejercicios 5 y 6 se encuentran agrupados debido a que trabajan sobre la misma estructura.

El **Ejercicio 6 utiliza como base el layout desarrollado en el Ejercicio 5**, agregando comportamiento responsive.

---

## EJERCICIO 5 — PÁGINA WEB CON GRID AREAS

Creación de una página web utilizando **Grid Areas**.

### Estructura

```text
┌─────────────────────────────────┐
│             HEADER              │
├────────────┬────────────────────┤
│            │                    │
│    MENU    │      CONTENT       │
│            │                    │
│            │                    │
├────────────┴────────────────────┤
│             FOOTER              │
└─────────────────────────────────┘
```

### Propiedades principales

```css
grid-template-columns;
grid-template-areas;
grid-area;
gap;
```

El objetivo es aprender a definir diferentes áreas dentro de una página y organizar los elementos mediante nombres.

---

## EJERCICIO 6 — RESPONSIVE

Este ejercicio parte de la página creada en el ejercicio anterior y adapta su estructura para dispositivos con pantallas pequeñas.

### Distribución en pantallas pequeñas

```text
┌──────────────────┐
│      HEADER      │
├──────────────────┤
│       MENU       │
├──────────────────┤
│     CONTENT      │
├──────────────────┤
│      FOOTER      │
└──────────────────┘
```

Para realizar la adaptación se utiliza una **Media Query** y se modifica la estructura de `grid-template-areas`.

```css
@media (max-width: 600px) {

    .pagina {
        grid-template-columns: 1fr;

        grid-template-areas:
            "header"
            "menu"
            "contenido"
            "footer";
    }
}
```

### Conceptos practicados

* Diseño responsive
* `@media`
* `grid-template-columns`
* `grid-template-areas`
* Adaptación del layout según el tamaño de pantalla

---

# ESTRUCTURA DEL PROYECTO

```text
EJERCICIOS-Estructura-HTML-Estilo-CSS/
│
├── Ejercicio1/
├── Ejercicio2/
├── Ejercicio3/
├── Ejercicio4/
├── Ejercicio5/
│
├── Layouts_Grid/
│   ├── ejercicio1Layouts_Grid/
│   ├── ejercicio2Layouts_Grid/
│   ├── ejercicio3Layouts_Grid/
│   ├── ejercicio4Layouts_Grid/
│   └── ejercicios5_6Layouts_Grid/
│
└── README.md
```

La carpeta `ejercicios5_6Layouts_Grid` contiene los ejercicios 5 y 6 debido a que ambos están relacionados directamente: el ejercicio 6 toma como base la estructura creada en el ejercicio 5 para implementar el diseño responsive.

---

# OBJETIVOS DE APRENDIZAJE

A través de estos ejercicios se busca desarrollar práctica en:

* Creación de estructuras HTML.
* Aplicación de estilos con CSS.
* Uso de CSS Grid.
* Definición de columnas y filas.
* Distribución de elementos dentro de un Grid.
* Uso de `grid-column`.
* Implementación de Grid Areas.
* Creación de layouts organizados.
* Uso de pseudoclases como `:hover`.
* Aplicación del Box Model.
* Diseño responsive mediante Media Queries.

---

# TECNOLOGÍAS

| Tecnología        | Uso                                   |
| ----------------- | ------------------------------------- |
| **HTML5**         | Estructura y contenido de las páginas |
| **CSS3**          | Estilos y presentación                |
| **CSS Grid**      | Creación y organización de layouts    |
| **Media Queries** | Adaptación responsive                 |

---

# ESTADO DEL PROYECTO

Proyecto realizado como parte del proceso de aprendizaje y práctica de **HTML5 y CSS3**, avanzando desde estructuras básicas hasta la creación de layouts mediante **CSS Grid y diseño responsive**.

---

> **Objetivo principal:** comprender cómo construir, organizar y adaptar estructuras web utilizando HTML y CSS.

## Autor

**Manuel Rodríguez González** 
