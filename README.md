# Jóvenes MIBAFUCA — Juegos

Juegos para las competencias de jóvenes de la iglesia MIBAFUCA.

## 100 Cristianos Dijeron

Versión cristiana de *100 Latinos Dijeron* (Family Feud), pensada para dos equipos y un presentador que controla todo desde una sola pantalla.

Hay dos versiones con la misma lógica de juego; elige la que más les guste:

| Versión | Estilo | Jugar en línea |
|---|---|---|
| **Versión 1** | Tablero clásico en columna, azul y dorado | https://hellenp-a.github.io/JOVENESMIBAFUCA/100-cristianos-dijeron.html |
| **Versión 2 (recomendada)** | Set de TV: hexágono dorado, tablero de dos columnas, PUNTOS y ERRORES por equipo, pulsador en el podio, casilla para escribir la respuesta con verificación automática, 100 preguntas + 30 extra | https://hellenp-a.github.io/JOVENESMIBAFUCA/100-cristianos-dijeron-v2.html |

**Jugar sin internet:** descarga el archivo `.html` de la versión que quieras y ábrelo con doble clic en Chrome, Edge o Safari.

### Cómo se juega

1. **Equipos:** por defecto *Guerreros de la Fe* y *JASAK*. Se cambian con el botón **Nombres de equipos** antes de empezar (en la Versión 2 no se editan durante el juego). Tocar el panel de un equipo le da el turno y se muestra el letrero grande "EN TURNO".
2. **Enfrentamiento (pulsador):** el presentador lee la pregunta y pulsa el botón rojo (o barra espaciadora). Un jugador de cada equipo está frente al teclado: el primero que presione **A** (equipo izquierdo) o **L** (equipo derecho) responde primero; luego responde el otro. El presentador escribe cada respuesta y el sistema la revela. **El presentador toca el panel del equipo cuya respuesta tuvo más puntos**: ese equipo queda "EN TURNO" e inicia el juego.
3. **Ronda:** el equipo en turno sigue diciendo respuestas. El presentador escribe cada una en la casilla bajo el tablero y pulsa Enter (no importan mayúsculas, tildes ni errores pequeños): si está, se voltea con su posición y puntos; si no está, aparece una X gigante, se enciende una X en ERRORES de ese equipo y **el turno pasa automáticamente al otro equipo**, que continúa hasta fallar. También existe el **Panel del juez** (ventana aparte con las 8 respuestas) para revelar con un clic.
4. **Turno:** por defecto el turno cambia con cada fallo. Con el botón "Turno cambia" se puede pasar al modo TV: tres errores y el otro equipo tiene una oportunidad de robo.
5. **Puntos:** botón "Puntos para…" o teclas **Q** (equipo izquierdo) y **P** (equipo derecho).
6. **Multiplicador:** x2 o x3 para que las últimas rondas valgan más.

### Atajos de teclado

| Tecla | Acción |
|---|---|
| Espacio | Activar el pulsador (enfrentamiento) |
| A / L | Pulsador del equipo izquierdo / derecho |
| 1–8 | Revelar respuesta a mano |
| X | Strike |
| Q / P | Dar puntos al equipo izquierdo / derecho |
| R | Revelar todas las respuestas |
| ← / → | Pregunta anterior / siguiente |
| Esc | Cerrar ventanas |

### Consejos para el día del evento

- Usa dos pantallas: en Windows pulsa **Win+P → Extender** (en Mac, Preferencias → Pantallas → desactivar duplicado). Deja el tablero en el proyector (F11 para pantalla completa) y el Panel del juez en la pantalla de la laptop, así el público no ve las respuestas.
- Si el navegador bloquea la ventana del panel, se abre debajo del tablero; en ese caso el juez puede girar la laptop o permitir ventanas emergentes para el sitio.
- Sube el volumen: los aciertos y strikes tienen sonido.
- Los marcadores se guardan en el navegador hasta pulsar **Reiniciar**.
- La Versión 2 trae 100 preguntas principales (1–100) y 30 extra (101–130) de temas generales para practicar y aprender la app antes del evento. El botón **Lista** permite saltar a cualquiera y marca las ya jugadas.

### Editar preguntas

Abre el archivo HTML con un editor de texto y busca `const QUESTIONS`. Cada pregunta tiene la forma:

```js
{"q":"Texto de la pregunta","c":"B","a":[["Respuesta mas popular",30],["Otra",20],["Otra",14],["Otra",11],["Otra",9],["Otra",7],["Otra",5],["Otra",4]]}
```

`"c":"B"` es pregunta principal y `"c":"X"` es extra. Cada pregunta tiene 8 respuestas ordenadas de la más popular a la menos popular y los puntos suman 100. Los sinónimos se escriben separados por " / " (ej. `"Ranas / Sapos"`) para que el verificador los acepte.
