# Jóvenes MIBAFUCA — Juegos

Juegos para las competencias de jóvenes de la iglesia MIBAFUCA.

## 100 Cristianos Dijeron

Versión cristiana de *100 Latinos Dijeron* (Family Feud), pensada para dos equipos y un presentador que controla todo desde una sola pantalla.

**Jugar en línea:** https://hellenp-a.github.io/JOVENESMIBAFUCA/100-cristianos-dijeron.html

**Jugar sin internet:** descarga `100-cristianos-dijeron.html` y ábrelo con doble clic en Chrome, Edge o Safari.

### Cómo se juega

1. **Equipos:** por defecto *Guerreros de la Fe* y *JAZAKM*. Haz clic sobre el nombre para cambiarlo. Haz clic en la tarjeta del equipo para marcar quién tiene el turno.
2. **Enfrentamiento:** un jugador de cada equipo responde; quien dé la respuesta más alta decide si su equipo juega o pasa.
3. **Ronda:** el jugador dice una respuesta. El juez pulsa **Revisar respuesta (panel del juez)**: se abre una ventana aparte con las 8 respuestas y sus puntos, que solo ve el juez en la laptop. Si la palabra está en la lista, pulsa esa respuesta y se revela en el tablero con su posición y puntos. Si no está, pulsa **No está en la lista** y se marca un strike. También se puede revelar a mano con clic o teclas 1–8.
4. **Turno:** con "Turno cambia: cada fallo" (por defecto) el turno pasa al otro equipo con cada respuesta que no está en la lista. Con "Turno cambia: 3 strikes" se juega como en la TV: tres fallos y el otro equipo tiene una oportunidad de robo.
5. **Puntos:** botón "Puntos para…" o teclas **Q** (equipo izquierdo) y **P** (equipo derecho).
6. **Multiplicador:** x2 o x3 para que las últimas rondas valgan más.

### Atajos de teclado

| Tecla | Acción |
|---|---|
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
- El banco tiene 20 preguntas; el botón **Lista** permite saltar a cualquiera y marca las ya jugadas.

### Editar preguntas

Abre el archivo HTML con un editor de texto y busca `const QUESTIONS`. Cada pregunta tiene la forma:

```js
{q:"Texto de la pregunta", a:[["Respuesta más popular",40],["Otra",25],["Otra",15]]}
```

Cada pregunta tiene 8 respuestas y los puntos suman 100 o menos. Los sinónimos se escriben separados por " / " (ej. `"Ranas / Sapos"`) para que el verificador los acepte.
