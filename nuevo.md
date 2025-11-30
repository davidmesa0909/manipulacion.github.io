# Aula Virtual BPM: Prevención de Enfermedades Transmitidas por Alimentos (ETA)

Este proyecto es una aplicación web educativa de **un solo archivo (Single File Application)** diseñada para reforzar los conocimientos del "Módulo de Capacitación 7" sobre seguridad alimentaria, higiene y control de temperaturas.

## 📋 Descripción

La aplicación es una herramienta interactiva que gamifica la evaluación de conocimientos críticos sobre inocuidad alimentaria. Está basada estrictamente en el material de capacitación proporcionado, cubriendo desde definiciones básicas hasta normativas técnicas de temperatura.

### Objetivos de Aprendizaje
El usuario podrá practicar y validar sus conocimientos en:
* [cite_start]**Definiciones de ETA:** Diferencia entre infección e intoxicación[cite: 11].
* [cite_start]**Epidemiología:** Datos sobre brotes en Colombia (2018) y alimentos de riesgo[cite: 7, 8].
* [cite_start]**Higiene:** Técnicas de lavado de manos y prevención de contaminación cruzada[cite: 35, 51].
* [cite_start]**Control de Procesos:** Temperaturas críticas de cocción y almacenamiento[cite: 70, 71, 72].

## 🎮 Módulos de Juego

La aplicación cuenta con tres actividades pedagógicas distintas:

1.  **Trivia Maestra (Quiz):**
    * Preguntas de selección múltiple sobre conceptos teóricos y estadísticas.
    * [cite_start]*Ejemplo:* Identificar el tiempo correcto de lavado de manos (20 segundos)[cite: 37].

2.  **Escenarios de Decisión (Verdadero/Falso - Casos):**
    * El usuario se enfrenta a situaciones cotidianas en una cocina.
    * [cite_start]*Ejemplo:* Decidir si lavar o no el pollo crudo (Práctica prohibida para evitar salpicaduras)[cite: 62].

3.  **Desafío de Temperaturas:**
    * Juego de emparejamiento para relacionar alimentos con su temperatura interna segura.
    * [cite_start]*Datos clave:* Aves a $165^\circ F$, Carne molida a $160^\circ F$, Cortes enteros a $145^\circ F$[cite: 70, 71, 72].

## 🛠️ Ficha Técnica

* **Tecnologías:** HTML5, CSS3, JavaScript (Vanilla).
* **Dependencias:** Ninguna. No requiere conexión a internet ni librerías externas.
* **Compatibilidad:** Funciona en cualquier navegador moderno (Chrome, Firefox, Edge, Safari).
* **Diseño:** Responsivo (adaptable a móviles y escritorio).

## 🚀 Instrucciones de Uso

1.  Descarga el archivo `entrenamiento_bpm.html`.
2.  Haz doble clic en el archivo para abrirlo en tu navegador web predeterminado.
3.  Navega a través del menú principal para seleccionar los minijuegos.

## ⚙️ Personalización (Para Desarrolladores/Instructores)

Todo el código se encuentra en un solo archivo para facilitar su transporte. Si deseas agregar más preguntas, busca la sección `<script>` al final del archivo HTML.

Encontrarás tres arreglos (arrays) de datos que puedes editar:

* `const quizData`: Para agregar preguntas a la Trivia.
* `const decisionData`: Para agregar nuevos escenarios de higiene.
* `const tempData`: Para modificar los ejercicios de temperatura.

**Ejemplo de estructura para agregar una pregunta:**

```javascript
{
    q: "¿Nueva pregunta?",
    options: ["Opción A", "Opción B", "Opción C"],
    answer: 0, // Índice de la respuesta correcta (0 es A, 1 es B...)
    feedback: "Explicación pedagógica que aparece al responder."
}