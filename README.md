# Riksdag 2026 – Sannolikhetskalkylator för Emil Steen (#5 M Östergötland)

En mobilanpassad single-page webbapplikation (HTML5, Tailwind CSS via CDN, Vanilla JavaScript) som beräknar och visualiserar sannolikheten för att **Emil Steen** (kandidat #5 för Moderaterna i Östergötlands läns valkrets) tillträder som tjänstgörande riksdagsledamot under mandatperioden 2026–2030.

Appen kan hostas direkt på **GitHub Pages** utan något build-steg.

---

## Funktioner

- **Sainte-Laguës jämkade uddatalsmetod**: Exakt beräkning av Östergötlands 14 fasta mandat + 3 utjämningsmandat (delare: 1.2, 3, 5, 7, 9...).
- **4,0 %-spärren**: Simulering av riksdagsspärren där partier under 4,0 % (särskilt Liberalerna L) nollställs och deras mandat omfördelas till de större partierna.
- **Konstitutionell ersättarkedja**:
  - Andreas Norlén (plats 1) avstår ordinarie ledamotsuppdrag för fortsatt uppdrag som Riksdagens talman eller statsråd.
  - Vid 4 M-mandat kliver Emil Steen in som **tjänstgörande ledamot från Dag 1** (100% chans).
  - Vid 3 M-mandat kliver Magdalena Hermelin in som talmansersättare och Emil Steen blir **1:e aktive ersättare** (45% chans över 4 år).
- **Duellmodul (M vs SD)**: Jämför M:s och SD:s jämförelsetal vid delare 7 och visar marginalen i både procentenheter och röster.
- **Interaktiv SVG-mätare (Gauge)**: Visar realtidsberäknad sannolikhet och dynamisk statusbadge.
- **Snabbscenarier (Presets)**: Valet 2022, Senaste opinionsmätning (Indikator Opinion), M tar 4 mandat, SD-duell, L över/under 4%.
- **Dela & Spara**: Alla slider- och reglagelägen synkroniseras automatiskt i webbadressens URL-hash.
- **Mobilanpassad & Responsiv**: Optimerad för smartphones med micro-steppers (+/- 0.1%), tydliga touchytor och mörkt Moderat-tema.

---

## Installation & GitHub Pages

Inga beroenden eller byggverktyg behövs (Tailwind CSS, Lucide Icons och Canvas Confetti laddas via CDN).

1. Klona repot:
   ```bash
   git clone https://github.com/DITT-ANVÄNDARNAMN/riksdag26.git
   ```
2. Öppna `index.html` direkt i valfri webbläsare.
3. För att aktivera GitHub Pages:
   - Gå till **Settings** -> **Pages** i GitHub-repot.
   - Välj `main` branch och root `/` som källa.
   - Spara – applikationen är live på några sekunder!
