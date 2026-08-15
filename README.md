# 📱 MenuApp - Suite de Bienestar y Entretenimiento
### *Proyecto de Programación Orientada a Objetos (Equipo Maravilla)*

**MenuApp** es una aplicación Android modular que integra herramientas de productividad personal, seguimiento de hábitos saludables y una colección de juegos clásicos para el entrenamiento mental. Este proyecto demuestra la implementación de principios de **POO**, manejo de persistencia de datos y diseño de interfaces en Android.

---

## ✨ Módulos Principales

La aplicación se divide en 4 pilares fundamentales accesibles desde un menú principal interactivo:

### 1. 📅 Productividad y Enfoque
* **Gestor de Actividades:** Sistema CRUD (Crear, Leer, Actualizar, Eliminar) para organizar tareas académicas y personales.
* **Temporizador de Enfoque:** Herramienta visual para sesiones de trabajo (estilo Pomodoro) con barra de progreso circular personalizada.

### 2. 💧 Bienestar y Salud
* **Control de Hidratación:** Registro diario de consumo de agua. Permite agregar vasos y visualizar el progreso hacia la meta diaria.

### 3. 🌱 Sostenibilidad
* **Registro Ecológico:** Módulo dedicado a registrar acciones sostenibles (como reciclaje o ahorro de energía) para fomentar hábitos positivos con el medio ambiente.

### 4. 🎮 Zona de Juegos (Brain Training)
Una colección de minijuegos implementados con lógica propia:
* **🧩 Puzzle Deslizante:** Rompecabezas lógico de ordenamiento numérico/visual.
* **🧠 Juego de Memoria:** Clásico juego de encontrar parejas de cartas.
* **💣 Buscaminas:** Implementación del clásico de estrategia con celdas y banderas.
* **❌⭕ Tres en Raya:** Juego de estrategia rápida para dos jugadores (o vs CPU).

---

## 🛠️ Tecnologías y Arquitectura

* **Lenguaje:** Java (Android SDK).
* **Build System:** Gradle (Kotlin DSL).
* **UI/UX:** XML Layouts, Material Design Components, Custom Drawables (gradientes, botones redondeados).
* **Persistencia:** Repositorios locales (`RepositorioActividades`, `RepositorioHidratacion`, etc.) y `GestorSesion` para manejo de preferencias de usuario.
* **Multimedia:** Integración de efectos de sonido (`ost1.mp3`, `ost2.mp3`) para mejorar la experiencia de usuario.

---

## 📂 Estructura del Proyecto

El código está organizado siguiendo una arquitectura limpia por paquetes:

```text
com.example.menuaplication/
│
├── data/               # Gestión de datos y Repositorios
│   ├── GestorSesion.java
│   └── Repositorio[Actividades/Agua/Sostenibilidad].java
│
├── model/              # Clases POJO y Lógica de Negocio
│   ├── actividades/    # Lógica de tareas y prioridades
│   ├── juegos/         # Lógica de Buscaminas, Puzzle, Memoria
│   └── ...
│
└── ui/                 # Interfaz de Usuario (Activities y Adapters)
    ├── menu/           # MainActivity, Login, Splash
    ├── actividades/    # CRUD de tareas y Timer
    ├── hidratacion/    # Tracking de agua
    ├── sostenibilidad/ # Tracking ecológico
    └── [juegos]/       # Activities de cada minijuego
```

---

## 👥 Equipo de Desarrollo

Este prototipo fue construido colaborativamente por:

- **José Paladines** (1Mejor2345)
- **Santiago Gómez** (SRGM-sys)
- **Matías Sánchez** (TheMattias1127)
- **Erwin Mora**     (Erwin-Mora)

Desarrollado para el **Proyecto de POO**
