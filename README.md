# WebGIS Inventarisasi Aset Jalan — Bobby

WebGIS interaktif untuk inventarisasi aset Penerangan Jalan Umum (PJU) dan Rambu Lalu Lintas, mencakup **Ruas 124–246**.

🗺 **Live:** [https://\<username\>.github.io/\<repo-name\>](https://github.io)

---

## Fitur

- **1.429 titik aset** — 1.250 PJU + 179 Rambu
- **121 ruas jalan** tercakup
- Klik titik → popup dengan **foto lapangan**
- Filter per ruas / jalan
- Toggle layer PJU & Rambu
- Basemap: OpenStreetMap & Satelit Esri
- Marker clustering otomatis

## Cara Deploy ke GitHub Pages

1. Fork / clone repo ini
2. Buka **Settings → Pages**
3. Source: **Deploy from a branch → main → / (root)**
4. Simpan — site akan live di `https://<username>.github.io/<repo-name>`

## Struktur Repo

```
├── index.html       # Aplikasi WebGIS utama
├── data.js          # Data semua 1.429 titik (koordinat, nama, tipe, ruas)
├── files/           # Foto lapangan (~2.980 file JPG)
└── README.md
```

## Data

Data bersumber dari survei lapangan KMZ:
- `PROGRESS BOBBY 124–173` (50 ruas)
- `Bobby Jilid 2 173–246`

## Teknologi

- [Leaflet.js](https://leafletjs.com/) — peta interaktif
- [Leaflet.markercluster](https://github.com/Leaflet/Leaflet.markercluster) — clustering marker
- OpenStreetMap & Esri World Imagery — basemap
- Vanilla HTML/CSS/JS — tanpa framework, tanpa build tools
