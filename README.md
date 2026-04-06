# Procesamiento de Imágenes en C (CLI)

[English version](./README.en.md) | **Español**
---

Este repositorio contiene un sistema desarrollado en lenguaje C para el procesamiento de imágenes BMP y PNM directamente desde la línea de comandos. El proyecto fue construido como parte de mi formación en programación estructurada, aplicando manejo de memoria, lógica modular y validación de entradas.

## 📌 Funcionalidades principales

- Separación de canales RGB (Rojo, Verde, Azul).
- Conversión de imágenes a escala de grises.
- Conversión a blanco y negro con umbral definido por el usuario.
- Generación de histogramas por canal y escala de grises.
- Mezcla de dos imágenes con coeficiente alpha ajustable.
- Menú de ayuda desde terminal con guía de comandos.

## 🛠️ Tecnologías y conceptos aplicados

- Lenguaje C.
- Archivos binarios (lectura/escritura BMP y PNM).
- Manejo de matrices tridimensionales.
- Argumentos desde consola (`argc` y `argv`).
- Modularización de funciones.
- Control de errores.

## 📁 Estructura del repositorio

```
├── FINAL_p.c               # Código fuente principal.
├── Pseudocodigo.txt        # Lógica del sistema en pseudocódigo.
├── README.md               # Documentación en español (este archivo).
├── README.en.md            # Documentación en inglés.
└── /outputs                # Imágenes BMP generadas (rojo, gris, bn, mezcla...).
```

## ▶️ Instrucciones de uso

### Compilación

```bash
gcc FINAL_p.c -o imagenes
```

### Comandos básicos

```bash
./imagenes 1b imagen.bmp                 # Separar RGB.
./imagenes 5b imagen.bmp                 # Escala de grises.
./imagenes 6b imagen.bmp 128             # Blanco y negro con umbral.
./imagenes 7b imagen.bmp                 # Generar histogramas.
./imagenes 8b frente.bmp fondo.bmp 100   # Mezcla con alpha.
./imagenes -help                         # Mostrar ayuda.
```

> Nota: funciona con imágenes BMP o PNM dependiendo del comando (`1b`, `1p`, etc.)

## 🧠 Aprendizajes clave

- Simulación de CLI para control de parámetros y procesos.
- Manipulación de archivos binarios en lenguaje C.
- Programación orientada a funciones reutilizables.
- Aplicación de estructuras y control de flujo.

## 📄 Licencia

Este proyecto fue realizado con fines educativos. Puedes reutilizar el código siempre y cuando cites la fuente y no uses con fines comerciales sin permiso.

## 👥 Créditos

Desarrollado por **Santiago Durán Rendón** – 2024.

Estudiante de Ingeniería en Computación – UNAM.

---