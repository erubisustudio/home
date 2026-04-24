# Design System Specification: Erubisu studio

# 🏺 Design System: The Digital Curator

Questo progetto adotta un approccio **Digital Curator**, ispirato al concetto giapponese di *Ma* (間) — l'uso intenzionale dello spazio vuoto. L'obiettivo è trasformare il portfolio in una monografia editoriale di alto livello, dove la precisione tecnica incontra l'eleganza fotografica.

## 🎯 Core Concept: Asymmetric Precision
Il design si basa su un contrasto dinamico: una griglia tecnica rigida che ospita layout organici, elementi sovrapposti e forti contrasti tipografici. 

---

## 🎨 Palette & Atmosfera (Wabi-Sabi Tones)
Ispirata a materiali naturali (lino, pietra, muschio, carbone).
- **Background Principale:** `#fafaf5` (Base)
- **Superfici Secondarie:** `#f3f4ee` (Low) / `#ecefe7` (Nesting)
- **Accenti Primari:** `#576246` (Seta/Foresta)
- **Testo (On-Surface):** `#2e342d` (Mai usare il nero puro #000)

### 🚫 La Regola "No-Line"
È vietato l'uso di bordi da 1px per separare le sezioni. La gerarchia visiva è definita esclusivamente dai **cambiamenti di colore di sfondo** e dal **folding** delle superfici.

---

## ✍️ Tipografia: Autorità Editoriale
Un dialogo tra arte e ingegneria attraverso l'uso di due font:
1.  **Noto Serif:** Per i titoli "Hero" (`display-lg`). Richiede ampio respiro (almeno 64px di margine).
2.  **Manrope:** Per il corpo del testo e i dati funzionali. Neutro, pulito, architettonico.
3.  **Micro-Copy:** Label tecniche in `on_surface_variant` con spaziatura espansa (`0.05em`) per un look "engineered".

---

## 🏗️ Principi di Elevazione (Tonal Layering)
Niente ombre aggressive. La profondità si ottiene tramite:
- **Stacking:** Sovrapposizione di toni diversi (es. carta bianca su fondo grigio lino).
- **Ambient Shadows:** Solo per elementi flottanti, ombre leggerissime e diffuse (`rgba(46, 52, 45, 0.06)`).
- **Glassmorphism:** Opacità al 70% e `24px` di sfocatura (backdrop-blur) per menu e modali.

---

## 🧩 Componenti Chiave
- **Buttons:** Angoli smussati (`0.5rem`), nessun effetto "pillola". Gradienti sottili (135°) per un finish setoso.
- **Cards:** Zero bordi. Utilizzo di `surface_container_low` e raggi di curvatura di `0.75rem` per le immagini.
- **Inputs:** Nessun box chiuso. Solo una linea di firma inferiore da 2px in `primary` nello stato attivo.
- **Gallery Scroller:** Scrollbar personalizzata come elemento di design (non default del browser).

---

## ✅ Do's & ❌ Don'ts
- **DO:** Abbraccia l'asimmetria. Usa lo spazio vuoto (anche 200px) come elemento attivo.
- **DO:** Accosta fotografia organica a tipografia tecnica e rigorosa.
- **DON'T:** Non affollare i margini (minimo `5vw` di safe area).
- **DON'T:** Non usare bordi o divisori. Usa il colore e il padding.
- **DON'T:** Non usare il nero puro; preferisci toni carbone caldi per il testo.
