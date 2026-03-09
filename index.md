lo---
marp: true
theme: gaia
class: invert
paginate: true
---

<style>
  /* Importamos fuentes: VT323 para el look Minecraft y Press Start 2P para títulos */
  @import url('https://fonts.googleapis.com/css2?family=Press+Start+2P&family=VT323&display=swap');

  section {
    font-family: 'VT323', monospace;
    font-size: 30px;
    background-color: #1a1a1a;
    background-image: url('https://www.transparenttextures.com/patterns/dark-matter.png');
  }

  h1, h2 {
    font-family: 'Press Start 2P', cursive;
    color: #55FF55; /* Verde Lima Minecraft */
    text-shadow: 4px 4px #000;
    text-transform: uppercase;
    font-size: 1.8rem;
  }

  /* Caja de texto estilo pergamino/libro */
  .mc-box {
    border: 4px solid #373737;
    background: #c6c6c6;
    color: #373737;
    padding: 20px;
    border-radius: 0px;
    box-shadow: 8px 8px 0px #000;
    margin: 10px 0;
  }

  /* Botones estilo Minecraft UI */
  button {
    font-family: 'VT323', monospace;
    font-size: 24px;
    background: #8b8b8b;
    color: white;
    border: 4px solid #000;
    border-top-color: #bdbdbd;
    border-left-color: #bdbdbd;
    padding: 10px 20px;
    cursor: pointer;
    margin: 5px;
  }

  button:hover {
    background: #3c8527; /* Verde cuando pasas el mouse */
    border-top-color: #55ff55;
    border-left-color: #55ff55;
  }

  #reloj { 
    color: #ffaa00; 
    font-family: 'Press Start 2P', cursive;
    font-size: 1.2rem;
    display: block;
    margin: 10px 0;
  }

  .res-msg { font-family: 'Press Start 2P', cursive; font-size: 1rem; margin-top: 15px; }
</style>

# ⛏️ Misión 01: El Nether
### Nivel de Dificultad: Survival

---

## 📖 RETO: LECTURA VELOZ
*Lee antes de que se agote el tiempo:*

<div class="mc-box">
  "UN GHAST ESTÁ SOBREVOLANDO EL LAGO DE LAVA. SI LOGRAS LEER ESTAS LÍNEAS SIN EQUIVOCARTE, PODRÁS ACTIVAR TU ESCUDO Y REFLEJAR SUS BOLAS DE FUEGO. ¡DATE PRISA, EL PORTAL DE REGRESO SE ESTÁ CERRANDO!"
</div>

<span id="reloj">00.00s</span>
<button onclick="window.startTime = performance.now(); window.timerInterval = setInterval(() => { document.getElementById('reloj').innerText = ((performance.now() - window.startTime)/1000).toFixed(2) + 's'; }, 10)">[ INICIAR ]</button>
<button onclick="clearInterval(window.timerInterval)">[ DETENER ]</button>

---

## ✍️ RETO: DICTADO
*Escribe en tu cuaderno lo que Papá te indique:*

![bg right:40% w:400](img/portal_anim.gif)

**Instrucción de Dictado:**
*(Notas para Papá: "Para sobrevivir en el Nether, es obligatorio llevar al menos una pieza de armadura de oro para que los Piglins no te ataquen.")*

---

## 🧠 RETO: COMPRENSIÓN
*¿Qué pasa si intentas dormir en una cama en el Nether?*

<br>

<button onclick="document.getElementById('res').innerText='❌ ¡BOOM! LA CAMA EXPLOTA.'; document.getElementById('res').style.color='#ff5555'">A) EXPOLOTA</button>

<button onclick="document.getElementById('res').innerText='❌ NO, ESO ES EN EL OVERWORLD.'; document.getElementById('res').style.color='#ff5555'">B) TE DUERMES</button>

<button onclick="document.getElementById('res').innerText='💎 ¡CORRECTO! +1000 XP'; document.getElementById('res').style.color='#55ff55'">C) EXPLOTA</button>

<div id="res" class="res-msg">---</div>

---

# 🏆 FIN DE LA SESIÓN
### RESULTADOS PARA EL CSV:

* **Velocidad:** Ver tiempo en Slide 2.
* **Dictado:** Evaluar ortografía (Oro, Nether, Piglins).
* **Comprensión:** ¿Cazó el error de ortografía en la opción A?

---

### Ajustes finales importantes:
1.  **YAML:** Asegúrate de que el comando de Docker en tu `.github/workflows/deploy.yml` sea exactamente:
    `marpteam/marp-cli index.md --html -o index.html`
2.  **Imágenes:** He usado GIFs y PNGs directos de la Wiki de Minecraft para que se vea más real.
3.  **Ortografía:** En el Quiz puse "Expolota" en la A y "Explota" en la C. Es un buen truco para su comprensión lectora ver si nota la diferencia antes de elegir.

¿Te gustaría que te ayude con el siguiente tema de "Monstruos Marinos" usando este mismo estilo de fuentes y botones pero con colores azules? Sería genial para armar tu carpeta de `/temas`.
