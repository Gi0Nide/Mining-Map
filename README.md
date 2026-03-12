# Μεταλλευτικός Χάρτης Ελλάδας — Leaflet Edition 🇬🇷🗺️

Διαδραστικός χάρτης με πραγματικά map tiles (CARTO Dark), zoom, pan, και 35 μεταλλευτικές τοποθεσίες.

**Website:** [oryktosploutos.net](https://www.oryktosploutos.net/)

---

## Γρήγορη Εκκίνηση

```bash
cd mining-map-leaflet-project
npm install
npm run dev
```

Ανοίγει στο `http://localhost:3001`

## Build & Deploy

```bash
npm run build
vercel --prod
```

## Ενσωμάτωση στο WordPress

```html
<iframe src="https://your-leaflet-map.vercel.app"
        width="100%" height="700px"
        style="border:none; border-radius:8px;"
        title="Μεταλλευτικός Χάρτης Ελλάδας">
</iframe>
```

## Δομή

```
mining-map-leaflet-project/
├── index.html
├── package.json            ← React 18 + Vite 6 + Leaflet 1.9
├── vite.config.js
├── public/favicon.svg
├── src/
│   ├── main.jsx
│   ├── App.jsx
│   └── MiningMap.jsx       ← Leaflet χάρτης
└── README.md
```

## Διαφορά από SVG έκδοση

| | Leaflet | SVG |
|---|---------|-----|
| Map tiles | CARTO Dark (real maps) | Σχεδιασμένο περίγραμμα |
| Zoom | Smooth tile-based | Programmatic SVG |
| Offline | Χρειάζεται internet | Λειτουργεί offline |
| Βάρος | +200KB (leaflet) | Zero deps |

---

*oryktosploutos.net · Ελληνικός Ορυκτός Πλούτος · 2026*
