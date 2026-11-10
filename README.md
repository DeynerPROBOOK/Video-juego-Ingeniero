# 🎓 Ingeniero Quest: La misión de la RAM

Plataformero 2D arcade en un **único archivo HTML**, hecho con HTML5 Canvas, CSS y JavaScript vainilla. Sin dependencias, sin servidor y sin instalación.

Controlas a un estudiante de ingeniería que recorre el campus, derrota materias universitarias respondiendo preguntas, encuentra la **Memoria RAM** y abre la puerta de la **Facultad** para recibir su **Título Universitario**.

## 🎮 Cómo jugar

1. Descarga `ingeniero-quest.html`.
2. Ábrelo con doble clic en cualquier navegador moderno (Chrome, Firefox, Edge, Safari).
3. Pulsa **Enter** o el botón **JUGAR**.

### Controles

| Acción | Teclado |
|---|---|
| Mover a la izquierda | `←` o `A` |
| Mover a la derecha | `→` o `D` |
| Saltar | `↑`, `W` o `Espacio` |
| Responder una pregunta | Clic o teclas `1` a `4` |

En pantallas táctiles aparecen botones en pantalla para moverte y saltar.

## 🧩 Reglas

- Siete materias patrullan el mapa: **derivadas** (`d/dx`), **integrales** (`∫`), **bucles** `for` y **condicionales** `if`.
- Al tocar una, el juego se pausa y aparece una pregunta de opción múltiple.
  - ✅ **Aciertas:** la materia desaparece y sumas 100 puntos.
  - ❌ **Fallas:** pierdes una vida y te empujan hacia atrás.
- Empiezas con **5 vidas**. Caer a un foso también te quita una, y reapareces al inicio de ese tramo de suelo.
- La **Memoria RAM** está sobre la plataforma más alta del mapa. Al recogerla, la puerta de la Facultad se desbloquea.
- Entra a la Facultad con la RAM para ganar y ver tu certificado de **Título Universitario**.

## 🛠️ Personalizar el juego

Todo el código está comentado dentro del mismo archivo.

- **Preguntas:** edita el objeto `TYPES`. Cada pregunta tiene el formato `[pregunta, correcta, mala1, mala2, mala3]`.
- **Mapa:** modifica el arreglo `plats` (suelo y plataformas) y `enemySpots` (posición y tipo de enemigos).
- **Dificultad:** ajusta `lives` en `reset()` y las constantes de física `SPEED`, `JUMP` y `GRAV`.
- **Nuevas materias:** añade una entrada a `TYPES` con `label`, `name`, `color` y `qs`, y úsala en `enemySpots`.

## 📁 Estructura

```
.
├── ingeniero-quest.html   # El juego completo (HTML + CSS + JS)
└── README.md
```

## 🌐 Publicar en GitHub Pages

1. Renombra `ingeniero-quest.html` a `index.html`.
2. En el repositorio ve a **Settings → Pages**.
3. Elige la rama `main` y la carpeta `/ (root)`, y guarda.
4. Tu juego quedará disponible en `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`.

## 📄 Licencia

Proyecto de uso libre con fines educativos. Añade aquí la licencia que prefieras (por ejemplo, MIT).
