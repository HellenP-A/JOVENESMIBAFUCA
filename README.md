# Jóvenes MIBAFUCA — Juegos

Juegos para las competencias de jóvenes de la iglesia MIBAFUCA.

## 100 Cristianos Dijeron

Versión cristiana de *100 Latinos Dijeron* (Family Feud), pensada para dos equipos y un presentador que controla todo desde una sola pantalla.

**Jugar en línea:** https://hellenp-a.github.io/JOVENEVESMIBAFUCA/100-cristianos-dijeron.html

**Jugar sin internet:** descarga `100-cristianos-dijeron.html` y ábrelo con doble clic en Chrome, Edge o Safari.

### Cómo se juega

1. **Equipos:** por defecto *Guerreros de la Fe* y *JAZAKM*. Haz clic sobre el nombre para cambiarlo. Haz clic en la tarjeta del equipo para marcar quién tiene el turno.
2. **Enfrentamiento:** un jugador de cada equipo responde; quien dé la respuesta más alta decide si su equipo juega o pasa.
3. **Ronda:** el equipo en turno dice respuestas. Cada acierto se revela (clic en la casilla o teclas 1–8) y suma al marcador "En juego". Cada fallo es un strike (tecla X).
4. **Robo:** con 3 strikes, el otro equipo tiene una sola oportunidad. Si acierta, se le dan los puntos; si falla, van al equipo original.
5. **Puntos:** botón "Puntos →" o teclas **Q** (equipo izquierdo) y **P** (equipo derecho).
6. **Multiplicador:** ×2 o ×3 para que las últimas rondas valgan más.

### Atajos de teclado

| Tecla | Acción |
|---|---|
| 1–8 | Revelar respuesta |
| X | Strike |
| Q / P | Dar puntos al equipo izquierdo / derecho |
| R | Revelar todas las respuestas |
| ← / → | Pregunta anterior / siguiente |
| Esc | Cerrar ventanas |

### Consejos para el día del evento

- Abre el juego en la laptop conectada al proyector y pulsa **F11** para pantalla completa.
- Sube el volumen: los aciertos y strikes tienen sonido.
- Los marcadores se guardan en el navegador hasta pulsar **Reiniciar**.
- El banco tiene 20 preguntas; el botón **Lista** permite saltar a cualquiera y marca las ya jugadas.

### Editar preguntas

Abre el archivo HTML con un editor de texto y busca `const QUESTIONS`. Cada pregunta tiene la forma:

```js
{q:"Texto de la pregunta", a:[["Respuesta más popular",40],["Otra",25],["Otra",15]]}
```

Los puntos de cada pregunta deben sumar 100 o menos. Máximo 8 respuestas por pregunta.
