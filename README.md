<!-- ========================================================= -->
<!-- ======================= ROUTIX README =================== -->
<!-- ========================================================= -->

<p align="center">
  <h1 align="center">🚛 ROUTIX 🤖</h1>
  <p align="center"><strong>Asistente de Planeación Operativa con IA para Transporte</strong></p>
  <p align="center">TRAXIÓN · Hackatón Bécalos Tech Challenge 2025</p>
</p>

<p align="center">
  <a href="https://chatgpt.com/g/g-69683d7260048191ac23075ebc4c23ea-routix">
    <img src="https://img.shields.io/badge/🤖%20Probar%20Agente-ROUTIX-blueviolet?style=for-the-badge" alt="Probar Agente ROUTIX">
  </a>
  <a href="https://drive.google.com/file/d/1xxrH30FJug5VJ7zCPBuzqLiV1R_mlnPz/view?usp=sharing">
    <img src="https://img.shields.io/badge/📄%20Ver%20Documentación-PDF-success?style=for-the-badge" alt="Ver PDF del Proyecto">
  </a>
</p>


---

## 🌟 ¿Qué es ROUTIX?

**ROUTIX** es un **agente de Inteligencia Artificial conversacional** diseñado para **estandarizar la planeación operativa inicial** de:

- 🚛 **Transporte de Carga**
- 🚌 **Transporte de Personal**

En solo **5 preguntas**, ROUTIX genera una **propuesta clara, explicable y accionable**, incluso cuando la información es incompleta.

> 🧠 *ROUTIX no reemplaza al coordinador operativo.*  
> ⚙️ *Estandariza su forma de pensar para reducir improvisación y retrabajo.*

---

## 🔗 Accesos rápidos

- 🤖 **Agente ROUTIX (Custom GPT)**  
  👉 https://chatgpt.com/g/g-69683d7260048191ac23075ebc4c23ea-routix

- 📘 **Documento completo del proyecto (PDF)**  
  👉 https://drive.google.com/file/d/1xxrH30FJug5VJ7zCPBuzqLiV1R_mlnPz/view?usp=sharing

---

## 🚀 ¿Qué problemas resuelve?

❌ Planeaciones improvisadas o inconsistentes  
❌ Exceso de preguntas y fricción con el usuario  
❌ Bloqueo por información parcial  
❌ Rutas sin trazabilidad ni criterio estandarizado  
❌ Retrabajo entre áreas operativas y comerciales  

✅ ROUTIX lo convierte en decisiones claras **desde el minuto uno**.

---

## ⚙️ ¿Qué es capaz de hacer ROUTIX?

### 🧭 Planeación inteligente (mínima y ordenada)
- Hace **Pregunta 0** para identificar el servicio (Carga / Personal)
- Luego realiza **exactamente 5 preguntas** clave (sin redundancias)
- No pide datos técnicos innecesarios
- Confirma en 1 línea lo que entendió y continúa (estilo operador-a-operador)

### 🚛 Transporte de Carga
- ✅ Define estructura de ruta: **Directa / Multi-parada / Dividida**
- ✅ Sugiere unidad: **3.5t / Rabón / Torton / Tráiler**
- ✅ Estima ocupación aproximada
- ✅ Maneja riesgo por tipo de carga (general, perecedera, peligrosa, alto valor)

### 🚌 Transporte de Personal
- ✅ Define capacidad por pasajeros y perfil (operativos, administrativos, ejecutivos, estudiantes)
- ✅ Sugiere unidad: **Van / Sprinter / Autobús / Ejecutivo**
- ✅ Ajusta por horarios de turno y prioridad del servicio

### 🧠 Razonamiento explicable y controlado
- ✅ Aplica reglas operativas (heurísticas) en lugar de “caja negra”
- ✅ Documenta supuestos con impacto: **Bajo / Medio / Alto**
- ✅ Calcula nivel de riesgo: **Bajo / Medio / Alto**
- ✅ Calcula nivel de confianza: **Alta / Media / Baja** según supuestos

### 🗺️ Google Maps automático (por orden)
- ✅ Genera link sin exigir que el usuario escriba “origen/destino”
- ✅ Usa el **orden de puntos**:
  - Primer punto → origin
  - Último punto → destination
  - Intermedios → waypoints
- ✅ Divide en 2 enlaces si hay demasiadas paradas

---

## 🧩 ¿Cómo funciona ROUTIX? (pipeline)

```text
Usuario
  ↓
Pregunta 0: Tipo de servicio (Carga / Personal)
  ↓
5 preguntas clave (mínimas)
  ↓
Chequeo de datos críticos
  ↓
Reglas operativas TRAXIÓN (heurísticas)
  ↓
Salida estandarizada (8 secciones)
  ↓
Ruta + Unidad + Riesgo + Confianza + Mapa


