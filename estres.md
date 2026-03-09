---
marp: true
theme: gaia
class: invert
paginate: true
---

<style>
  button { 
    background: #3e8e41; color: white; border: none; padding: 10px 20px; 
    border-radius: 5px; font-family: 'Courier New', monospace; cursor: pointer;
    margin: 5px;
  }
  button:active { background-color: #1e4d2b; }
  .fail-btn { background: #e74c3c; }
  #reloj { color: #f1c40f; font-weight: bold; font-family: 'Courier New'; }
  .st-box { border: 2px solid #555; padding: 15px; border-radius: 10px; background: #222; }
</style>

# ⛏️ Misión: Sobreviviendo a la Lectura
### Nivel: Bioma de Selva
**Objetivo:** Recolectar XP de conocimiento.

---

## 📖 Reto 1: El Portal en Ruinas
*Lee rápido antes de que los Piglins te vean:*

<div class="st-box">
  "Encontré un portal de obsidiana llorosa escondido bajo las raíces de un árbol gigante. Las leyendas dicen que si logras leer las inscripciones antiguas sin trabarte, el portal te llevará directo a un cofre lleno de diamantes y manzanas doradas."
</div>

### ⏱️ Cronómetro de Misión:
<span id="reloj">00.00</span> segundos
<button onclick="window.startTime = performance.now(); window.timerInterval = setInterval(() => { document.getElementById('reloj').innerText = ((performance.now() - window.startTime)/1000).toFixed(2); }, 10)">INICIAR</button>
<button onclick="clearInterval(window.timerInterval)">DETENER</button>

---

## ✍️ Reto 2: Forjando Herramientas
*Escribe en tu cuaderno las instrucciones del herrero:*

![bg right:40%](https://minecraft.wiki/images/Smithing_Table_JE3_BE2.png)

**Instrucción de Dictado:**
*(Papá lee las notas mientras tú preparas el lápiz)*

> **Pista:** ¡Cuidado con la ortografía, o la herramienta se romperá!

---

## 🧠 Reto 3: El Quiz del Creeper
*Si respondes mal... ¡BOOM!*

**¿Cuál de estos materiales es indispensable para activar un portal al Nether?**

A) Piedra y Madera.
B) Pedernal y Hierro.
C) Polvo de Redstone.

<div style="margin-top: 20px;">
  <button onclick="document.getElementById('res').innerText='❌ ¡Ssssss... BOOM! Intenta de nuevo.'; document.getElementById('res').style.color='#e74c3c'">A o C</button>
  <button onclick="document.getElementById('res').innerText='💎 ¡NIVEL COMPLETADO! +500 XP'; document.getElementById('res').style.color='#2ecc71'">Opción B</button>
</div>

<h2 id="res">---</h2>

---

# 📊 Resumen para Papá
*Anota los resultados en tu CSV:*

1. **Lectura:** Tiempo marcado en la Slide 2.
2. **Dictado:** Revisar puntos, comas y acentos.
3. **Comprensión:** ¿Lo logró al primer intento?

**¡Siguiente misión: Monstruos Marinos! (Próximamente)**