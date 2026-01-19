# 🎵 MusicOn - Sistema de Gestión Musical (C++ Backend)

> **Desarrollado como Proyecto Final de Programación II en UTN FRGP (2025).**

## 💡 Sobre el Proyecto
MusicOn es una aplicación de consola desarrollada en C++ diseñada para simular el backend de una plataforma de streaming de música. El sistema gestiona un catálogo completo de artistas, álbumes y canciones, además de administrar usuarios, suscripciones (Premium/Gratuito) y generar reportes estadísticos avanzados sobre el consumo de contenido.

El núcleo del proyecto es su **motor de persistencia personalizado**, diseñado para minimizar la redundancia de datos mediante la normalización de archivos binarios y el uso de claves foráneas lógicas.

---

## 🚀 Funcionalidades Principales

### 🎧 Gestión de Catálogo y Usuarios
* **ABM Completo:** Altas, bajas y modificaciones de Artistas, Álbumes, Canciones y Géneros.
* **Sistema de Suscripciones:** Gestión de usuarios con diferentes niveles de acceso (Gratuito, Premium).
* **Playlists:** Creación y gestión de listas de reproducción personalizadas (relación muchos a muchos).

### 📊 Motor de Reportes y Estadísticas
El sistema procesa el historial de reproducciones (`Accesos.dat`) para generar métricas de negocio en tiempo real:
* **Ranking de Canciones:** Top de temas más escuchados, filtrados por franjas etarias (1-15, 15-25, etc.).
* **Análisis de Géneros:** Identificación de tendencias musicales por periodo.
* **Top Usuarios:** Ranking de los suscriptores más activos y "Top Fans" de canciones específicas.
* **Métricas Anuales:** Desglose mensual de reproducciones para análisis de crecimiento.

### 🔍 Módulo de Consultas
Búsqueda optimizada de música y playlists por múltiples criterios (Nombre, Autor, Género, Año de lanzamiento).

---

## 🛠️ Aspectos Técnicos Destacados

Este proyecto demuestra el dominio de fundamentos de programación y estructuras de datos sin depender de frameworks de alto nivel:

* **Lenguaje:** C++ (Standard 11/14).
* **Persistencia de Datos:** Implementación propia de sistema de archivos binarios (`.dat`).
* **Arquitectura:** Diseño modular separado en archivos de cabecera (`.h`) e implementación (`.cpp`) para facilitar el mantenimiento.
* **Algoritmos:** Lógica propia para ordenamiento de rankings y filtrado de datos en memoria.
* **POO:** Uso extensivo de Clases, Herencia y encapsulamiento.

---

## 📂 Estructura de Datos (Persistencia)
El sistema utiliza una arquitectura normalizada para garantizar la integridad referencial:
* **Entidades Principales:** `Artistas.dat`, `Albumes.dat`, `Canciones.dat`, `Suscriptores.dat`.
* **Transaccional:** `Accesos.dat` (Log de reproducciones).
* **Asociativas:** `Listas_Canciones.dat` (Relación N:N entre Listas y Canciones).

---

## 💻 Instalación y Ejecución

1.  Clonar el repositorio:
    ```bash
    git clone [https://github.com/tu-usuario/musicon.git](https://github.com/tu-usuario/musicon.git)
    ```
2.  Abrir el proyecto `musicon.cbp` en Code::Blocks (o importar los archivos `.cpp` y `.h` en tu IDE de preferencia como Visual Studio o CLion).
3.  Compilar y ejecutar.
    * *Nota: El sistema generará automáticamente los archivos `.dat` si no existen.*

---

## 👥 Autores
* **Damian Ezequiel Defederico** - [Tu LinkedIn]
* **Tobias Locastro**
