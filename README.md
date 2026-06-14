# 🥏 WJUC 2026 Predictor — Desde La Línea

Predictor interactivo para el **World Junior Ultimate Championships 2026**  
📍 Logroño, España · 11–18 Julio 2026

Creado por **Desde La Línea** — cobertura de Ultimate Frisbee en español.

🔗 **App en vivo:** [desdelalinea.github.io/wjuc2026-predictor](https://desdelalinea.github.io/Wjuc2026/)  
📲 **Instagram:** [@desdelalinea](https://instagram.com/desdelalinea)  
☕ **Ko-fi:** [ko-fi.com/desdelalinea](https://ko-fi.com/desdelalinea)

---

## ✨ Características

- **3 divisiones**: Open (19 equipos · 4 grupos), Women's (14 equipos · 2 grupos), Mixed (14 equipos · 2 grupos)
- **Picks de grupos y bracket** — selecciona ganadores de cada partido de grupos y avanza en el bracket
- **Spirit of the Game** — elige el equipo más espirituoso por división (+15 pts por acierto)
- **Leaderboard en tiempo real** con Firebase Firestore
- **Filtros**: General · Por País · LATAM · Por Club
- **Ranking por Club** — suma de puntos de todos los jugadores del mismo equipo
- **Auto-carga de picks** desde Firebase al volver a la app
- **Modo oscuro / claro**
- **Dark mode** por defecto, toggle manual
- **Multiidioma** — Español / Inglés
- **Exportación CSV** desde el panel admin
- **Sistema de patrocinadores** con carga de logos y publicación en Firestore

---

## 📊 Sistema de puntuación

| Acción | Puntos |
|--------|--------|
| Partido de grupos correcto | +1 pt |
| Equipo avanza al bracket | +2 pts |
| Cuartos de final (solo Open) | +5 pts |
| Semifinal correcta | +8 pts |
| Campeón correcto | +13 pts |
| Spirit of the Game (×3 divisiones) | +15 pts c/u |
| **Máximo total** | **304 pts** |

---

## 🏗 Arquitectura

```
index.html          ← App completa en un solo archivo
.nojekyll           ← Desactiva el procesado Jekyll de GitHub Pages
README.md           ← Este archivo
SETUP.md            ← Guía de configuración de Firebase
HOW-TO-PLAY.html    ← Página de instrucciones standalone
FIREBASE_RULES.txt  ← Reglas de seguridad de Firestore
LICENSE             ← MIT License
```

**Stack técnico:**
- HTML/CSS/JS puro — sin frameworks, sin build step
- [Firebase Firestore](https://firebase.google.com/) — leaderboard en tiempo real
- [GitHub Pages](https://pages.github.com/) — hosting gratuito

---

## ⚙️ Panel Admin

Accede desde la pestaña **⚙️ Admin** en la app.  

Desde el panel puedes:
- Ingresar resultados de partidos de grupos y bracket
- Publicar resultados para activar el leaderboard con puntos
- Registrar ganadores de Spirit of the Game
- Gestionar logos de patrocinadores
- Forzar apertura/cierre de picks
- Exportar CSV y JSON de participantes

---

## 📁 Datos del torneo

- **Fuente oficial**: [results.wfdf.sport](https://results.wfdf.sport/)
- **Referencia WJUC 2024**: Nottingham, GB (usada para badges históricos)
- **Grupos WJUC 2026** actualizados con seedings oficiales WFDF

---

## 📜 Licencia

MIT © 2026 Desde La Línea  
No Puedes usar, modificar y distribuir libremente.
